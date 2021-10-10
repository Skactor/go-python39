# go-python39 

Golang bindings for the C-API of CPython-3.9

Currently supports python-3.9 only.

Forked from [DataDog/go-python3](https://github.com/DataDog/go-python3)

Recommended using `asdf` to install Python

```
asdf plugin add python
asdf install python 3.9.7
```

So you can use the python library and headers without affecting the system python environment

Set the cgo flags to specify the python path before each go tool command

Example:

```bash
CGO_CFLAGS="-I /home/work/.asdf/installs/python/3.9.7/include/python3.9" \
CGO_LDFLAGS="/home/work/.asdf/installs/python/3.9.7/lib/libpython3.9.a" \
go run examples/python3/main.go
```

So you can see the same as ordinary Python interactive terminals as below

```
Python 3.9.7 (default, Oct 10 2021, 21:43:08) 
[GCC 11.1.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Rewrapping the library as you like!!!
