thunkous
========

Monkeypatch that lets you easily turn any async function or method into a thunk

Loosely based on [fibrous](https://github.com/goodeggs/fibrous)

Ex:
```js
    fs.thunk.readFile("/tmp/hello.txt", "utf8")
```
is the same as
```js
    require("thunkify")(fs.readFile)("/tmp/hello.txt", "utf8")
```
    
