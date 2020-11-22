# pybugger
A simple python debugger

## Code snippets and examples
```py
from debug import Debug

d = Debug()

d.variable('d', d)
```
Result: 
`[VARIABLE]: 'd' = <__main__.Debug object at HASH_ADDRESS>`

```py
d = Debug()

def foo(msg: str) -> None:
	d.function('foo', {'msg': msg})
	print(msg)
	
foo('Hello world')
```
Result:
```
[FUNCTION]: Executed 'foo' with 'msg: 'Hello world'' as arguments.
Hello World
```
