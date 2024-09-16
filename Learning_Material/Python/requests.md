# Requests Library
The `requests` library is a Python package for sending HTTP requests easily.
As a reminder, the HTTP protocol supports several request methods, including `HEAD, GET, POST, PUT, OPTIONS` and others.
Each of these methods structures the request slightly differently.
For example, in a GET request, the data you send to the server is typically passed as part of the URL, while in a POST request, the data is included in the request body.

The requests library wraps these HTTP requests in a very simple and user-friendly interface, abstracting away the complexity of manually handling connections.

Installing requests:
To get started, install the library by running this in your terminal:

```bash
pip install requests
```

Let's see some examples
Here’s a quick example of how you can use requests to send a simple GET request:
```python
import requests

response = requests.get('https://api.example.com/data')
if response.status_code == 200:
    print('Success!', response.json())  # get the response as JSON and print it
else:
    print('Error:', response.status_code)
```
And for a POST request, where you might send data in the body:

```python
import requests

data = {'key1': 'value1', 'key2': 'value2'}
response = requests.post('https://api.example.com/submit', data=data)

if response.status_code == 201:
    print('Yayyy it worked!')
else:
    print('Error:', response.status_code)
```
