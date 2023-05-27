# Document For asBASE

<b>Download it using pip:</b>
 ``` pip install asBASE ```
<pre></pre>
<b>On Pypi:</b>
* <a href="https://pypi.org/project/asBASE">asBASE</a>
<pre></pre>
# Simple example library with key value
```
from asBASE import asJSON

db = asJSON("as.json") # file_name

db.set("hi","hello")
print(db.get("hi"))
```
# To get key data:
```
key = db.get("key_name")
print(key)
```
# To delete a key and the data:
```
db.delete("key_name")
```
# To add a array or a list
```
db.sadd("hi","hello1")
db.sadd("hi","hello2")
```
# To get the content of a list or array
```
print(db.smembers("hi"))
```
# To make a temporary period for the key, and it expires after the period expires
```
db.expire("hi", 190) # Duration in seconds
```
# To see the time remaining until the key expires
```
print(db.ttl("hi"))
```
