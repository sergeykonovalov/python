# Flask

Flask use cases:

- static site with templates
- processing forms
- simple APIs
- chatbots with web hook

To run application:

- `python3 app.py`
- `flask run`
  - Looks for `app.py`, `wsgi.py` or value of `FLASK_APP` environment variable.
    - `export FLASK_APP='file.py'`
    - `$env:FLASK_APP='file.py'`
    - `set FLASK_APP='file.app'`

## Routing

- If you forget trailig slash, there will be redirect to URL with slash in the end.
- With arguments watch if you put trailing slash or not.
  - `/users/<username>` and `/users/<username>/` are different.

## Templates

It is just a folder, so not necessarily to be a Python module.

## Watching Changes

```shell
FLASK_ENV=development flask run
flask run --reload --debugger
```
