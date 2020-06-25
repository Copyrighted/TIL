# TIL

I was inspired by this hackernews thread https://bit.ly/2YaVdlh to write my own TIL repo.  I think it's important to keep a journal of knowledge you have acquired and interesting things you have found.  You can't remember everything, right?
I started this repo on 4/18/2020.  I want to clean it up to look like the original in the hackernews post.  Will do that in a bit.  **Some of this information isn't stuff I learned the day of but I think it's good to write down to cement it.**

### Awk in 20 minutes
[Learn AWK in 20 minutes.](https://ferd.ca/awk-in-20-minutes.html)

### Use url_for to get folder path for static content in Flask
This is a good stackoverflow post covering it. [Link to SO](https://stackoverflow.com/questions/16351826/link-to-flask-static-files-with-url-for)

### Visual map of the Linux Kernel

[Visual Map of Kernel](https://makelinux.github.io/kernel/map/)

### A good resource for cool stuff you can do with pipes

https://prithu.xyz/posts/unix-pipeline/

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
You should have a requirements.txt when using Django.  It makes it easier to deploy the application.