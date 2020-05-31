# TIL

I was inspired by this hackernews thread https://bit.ly/2YaVdlh to write my own TIL repo.  I think it's important to keep a journal of knowledge you have acquired.  You can't remember everything, right?
I started this repo on 4/18/2020.


### UIDS

If you need to generate random ID's for databases in python uuid.uuid4() is pretty useful.  Link: https://docs.python.org/3/library/uuid.html

### Markdown Editors

Markdown editors like summernote exists and allow you to embed them in web apps. Link: https://summernote.org/getting-started/#compiled-css-js

### WTF-Form Validation

Useful for learning why forms aren't being validated in Flask-WTF forms. Link: https://stackoverflow.com/questions/10722968/flask-wtf-validate-on-submit-is-never-executed

### PyCharm has it's own separate console

PyCharm has it's own console.  So if you're using functions like getpass() you probably wont be prompted for input in the console.
To fix this, do the following: edit configurations->emulate terminal ouput in console

### Flask CSRF

If you're using HTTP in a flask development environment, set SESSION_COOKIE_SECURE=False or else you'll get CSRF token missing.. a lot..
