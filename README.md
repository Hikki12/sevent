# Simple Event Emitter
Simple event emitter without dependencies.

## EXAMPLE
--------
```
from sevent import Emitter 
import time

def callback(message):
    print(message)

def do_something():
    time.sleep(1)

event = Emitter() 
event.on('ready', callback)
do_something()
event.emit('ready', 'Finished!')
```
## LICENSE
--------
MIT
