### flask
---
http://flask.pocoo.org/

```py
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello():
  return "Hello World!"
```

```sh
pip install Flask
FLASK_APP=hello.py flask run
```

```py 
from werkzeug.contrib.fixers import LighttpdCGIRootFix
app.wsgi_app = LighttpdCGIRootFix(app.wsgi_app)

```

