# Welcome to our first event 🥳🎈

### Disclaimer. 
The goal of this exercise is to understand complex and unclear code,                                          
and to improve your ability to read it, even if it comes from a colleague with unique working styles or approaches.


# let's start

I've written several functions here that may seem chaotic.               
Your task is to understand and use them to get the flag. Good luck!

```python

import random

LOWERCASE = 'abcdefu'


def megalol(x, **kwargs):
    return chr(ord(x) + kwargs.get('num', random.randint(1, 6)))

def theyseemerolin(n):
    return chr(n)

def theyhating(c):
    return ord(c)
    
def bomba(s, *args):
    def huge(*args):
        return s[slice(args[0], args[1])]
    return huge
    
def hexakill(h):
    return str(int(h, 16))
    
def makemedoit():
    return ''.join(chr(random.randint(67, 97)) for i in range(1, 9))
    
def hehe(s):
    return s[::-1][::-1]

def momo(t):
    return str(f'{t}{LOWERCASE[6]}').encode().decode()[0]

```
## THIS IS MY VICTORY MAP!

- megalol `Q` `3`
- theyseemerolin `104`
- hexakill `0x0F`
- bomba(makemedoit + `_15_Y0` + makemedoit) `8` `14`
- theyseemerolin theyhating `u`
- hehe `r_f`
- momo `l`
- hexakill `0x04`
- theyseemerolin `103`
