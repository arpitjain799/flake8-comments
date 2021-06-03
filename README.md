# flake8-comments

Report redundant comments in python code.

An example of a bad comment:

```python
# create user
user.create(force=True)
```

In this example, the comment gives even less information that the code itself. So, you can safely remove the comment without losing any information. The goal is to reduce the [information redundancy](https://en.wikipedia.org/wiki/Redundancy_(information_theory)), leaving in the code only what is actually important and helpful.

## Installation

```bash
python3 -m pip install flake8-comments
```

## Usage

Check that plugin was added in your flake8:

```bash
$ python3 -m flake8 --version
3.7.7 (flake8-comments: 0.1.0, mccabe: 0.6.1, pycodestyle: 2.5.0, pyflakes: 2.1.1) CPython 3.6.7 on Linux
```

If you don't see `flake8-comments` in the previous command output, check that `flake8` and `flake8-comments` is installed in the same interpreter.

If everything is OK, run `flake8`:

```bash
python -m flake8 example.py
```

## Similar projects

There are a few more good flake8 plugins targeted on cleaning up comments:

+ [flake8-eradicate](https://github.com/wemake-services/flake8-eradicate) detects commented out code.
+ [flake8-todos](https://github.com/orsinium-labs/flake8-todos) controls consistency of TODO comments.
+ [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) has a few checks targeted on comments, like if there are empty comments, too many `noqa`, `no cover`, bad shebangs.
