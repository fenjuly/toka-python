## Toka

[![Pypi version](https://img.shields.io/badge/pypi-v0.2.3.21-green.svg)](https://pypi.python.org/pypi/toka)
[![NPM download](https://img.shields.io/badge/download-v0.2.3.21-green.svg)](https://pypi.python.org/packages/source/t/toka/toka-0.2.3.21.tar.gz)

### A handy tool to generate common files in command line

This is python version related to this project [https://github.com/aprilorange/toka](https://github.com/aprilorange/toka).

```bash
pip install toka 

toka
toka -v
toka .gitignore <LAUNGUAGE NAMES>   # alias to toka g/git
toka .bowerrc <COMPONENT DIR>       # alias to toka b
toka license <LICENSE NAME>         # alias to toka l
toka webpack                        # alias to toka w
```

#### Arguments:

gitignore only:

- -d/--default : generate default file
- -a/--append : append to an existing file
- -g/--global : save to ~/.gitignore_global

webpack only:

- -p/--path
- -f/--filename
- -e/--entry

gulp only:

- -b/--babel : use gulpfile.babel.js

Example:

```bash
toka .gitignore -d
toka .gitignore python,go -a
toka .gitignore windows
toka .bowerrc lib
toka license MIT
toka gulp -b
toka webpack -e src/app/app.js -p /build/js -f bundle.js
```

The `.gitignore` languages we support: [Full List](lib/list/gitignore.js)

The LICENSE type we support:

(Fuzzy search is now supported! It means you can simply type things like `toka l apa` to add Apache license)

- Apache-2.0
- BSD-2
- BSD-3
- GPL-2.0
- ISC
- MIT
- MPL-2.0
- WTF

Yap, here we go and go happy.

## LICENSE

[MIT](LICENSE)
