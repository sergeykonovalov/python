# Virtual Environment

Python has built-in module `venv` [recommended for use](https://stackoverflow.com/questions/41573587/what-is-the-difference-between-venv-pyvenv-pyenv-virtualenv-virtualenvwrappe). Although Debian/Ubuntu moved this into separate package `python-venv`.

```shell
python3 -m venv .
source my-project/bin/activate
deactivate
```
