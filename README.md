# TIL

I was inspired by this hackernews [thread](https://news.ycombinator.com/item?id=22908044) to write my own TIL repo.  I think it's important to keep a journal of knowledge you have acquired and interesting things you have found.  You can't remember everything, right?
I started this repo on 4/18/2020.  I want to clean it up to look like the original in the hackernews post.  Will do that in a bit.  


### TIL Using pip3 and Travis CI
If you want to use pip3 with Travis CI use the [Trusty](https://docs.travis-ci.com/user/reference/trusty/#what-this-guide-covers) infrastructure.

### TIL Scoped Sessions in Flask
If you're running into errors such as 
"sqlite3.ProgrammingError: SQLite objects created in a thread can only be used in that same thread. The object was created in thread id 139900647581440 and this is thread id 139900760037184."
You can usually fix this by using scoped sessions in Flask.

[Link to relevant doc page](https://docs.sqlalchemy.org/en/13/orm/session.html?highlight=scoped_session#unitofwork-contextual)

### Undoing Git Add through command line
To undo git add through the command line use git reset.

### Awk in 20 minutes
[Learn AWK in 20 minutes.](https://ferd.ca/awk-in-20-minutes.html)

### Use url_for to get folder path for static content in Flask
This is a good stackoverflow post covering it. [Link to SO](https://stackoverflow.com/questions/16351826/link-to-flask-static-files-with-url-for)

### Visual map of the Linux Kernel

[Visual Map of Kernel](https://makelinux.github.io/kernel/map/)

### A good resource for cool stuff you can do with pipes

https://prithu.xyz/posts/unix-pipeline/

### Travis CI/CD
Easy way to have automatic testing when commiting to github repo [Travis CI](https://travis-ci.org/)

### UIDS

If you need to generate random ID's for databases in python uuid.uuid4().int is pretty useful.  [UUID Python Doc Link](https://docs.python.org/3/library/uuid.html)

### Markdown Editors

Markdown editors like [summernote](https://summernote.org/getting-started/#compiled-css-js) exists and allow you to embed them in web apps. 
Just remember to set the name in your html to whatever name you have for posts or submissions in your form.

In my forms.py
post = TextAreaField(validators=[]DataRequired()])

Now your textarea field should look like this

    <form method="POST">
        {{ form.hidden_tag() }}
        <label for="summernote"></label><textarea id="summernote" name="post"></textarea>
        <p>{{ form.submit() }}</p>
    </form>

### PyCharm has it's own separate console

PyCharm has it's own console.  So if you're using functions like getpass() you probably wont be prompted for input in the console.
To fix this, do the following: edit configurations->emulate terminal ouput in console

### Nice write-up about Flasks Application Factory and Application Context
I thought this was a nice write up about Flasks application factory and context.
[HackersAndSlackers Link](https://hackersandslackers.com/flask-application-factory)

### AJAX
AJAX is extremely useful because it allows you to update parts of your website using Javascript without having to refresh the page.


### Django Requirements
You should have a requirements.txt when using Django.  It makes it easier to deploy the application by having a list of dependencies.

### Idempotence and RESTful API's
What is idempotence?
The requests you make to a server dont change the resource state of the server.
 - Post is not idempotent.
 - GET, PUT, DELETE, HEAD,OPTIONS and TRACE are idempotent.
