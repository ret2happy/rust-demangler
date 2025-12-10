# rust_demangler

A package for demangling Rust symbols, written in Python.

Setup
-----
Install from GitHub using pip:
```bash
pip install git+https://github.com/ret2happy/rust-demangler.git
```

Or using uv:
```bash
uv add git+https://github.com/ret2happy/rust-demangler.git
```

Usage
-----
```py
from demangler import demangle
print(demangle(<mangled_name>))
```
Example 
-------
```py
demangle("_ZN3foo3barE") == "foo::bar"  #legacy style
demangle("_RNvC6_123foo3bar") == "123foo::bar"  #v0 style
```

License 
-------

This project is licensed under the [MIT License](LICENSE)
