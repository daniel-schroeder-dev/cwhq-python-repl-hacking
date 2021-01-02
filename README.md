# CWHQ Python REPL

A Python REPL for the kids at CWHQ. Built with [jQueryTerminal](https://terminal.jcubic.pl/) and [Pyodide](https://github.com/iodide-project/pyodide).

## Installation

It's just an HTML file, so download `index.html` to your machine and you're ready to go!

## Usage

It's a Python REPL, so use it like you would any other REPL. Several things don't work yet, as documented below in [Issues](issues).

## Issues

Currently, you can't enter multi-line `dicts`, `lists`, or `tuples`:

```text
>>> my_dict = {
Traceback (most recent call last):
  File "/lib/python3.8/site-packages/pyodide/_base.py", line 64, in eval_code
    mod = ast.parse(code)
  File "/lib/python3.8/ast.py", line 47, in parse
    return compile(source, filename, mode, flags,
  File "<unknown>", line 1
    my_dict = {
              ^
SyntaxError: unexpected EOF while parsing
>>> 
```

I'm sure there are many more issues, so if you find one, please let me know!

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
