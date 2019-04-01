
login:demo

pass:demo

# Under the hood:
- [Python](http://python.org/)
- [Flask](http://flask.pocoo.org/)
- [MongoDB](http://www.mongodb.org/)
- [Bootstrap 3](http://getbootstrap.com/)
- [jQuery](http://jquery.com)
- [Lightbox 2](https://github.com/lokesh/lightbox2)
- [Markdown](http://daringfireball.net/projects/markdown/syntax)
- [Polymer](http://www.polymer-project.org)


# What it can:
- create/preview/update/delete articles;
- create/update/delete users;
- search;
- atom feed.

# It contains:
- WYSIWYG Markdown editor;
- [AddThis](http://www.addthis.com/) social buttons;
- [Gravatar](http://gravatar.com) for userpic.


# Requirements:
- mongoDB >= 2.2


# Installation:
`git clone https://github.com/dmaslov/flask-blog.git`

`cd flask-blog`

`virtualenv --no-site-packages ./env`

`source ./env/bin/activate`

`pip install -r requirements.txt`


After this edit the `config.py` file

- Replace the `CONNECTION_STRING` variable with your own connection string;

- Replace the `DATABASE` variable to your own one;

- If the default collection names don't work for you please replace the `POSTS_COLLECTION`, `USERS_COLLECTION` and `USERS_COLLECTION` variables to any names you like;

- If you use this code on a production sever replace the `DEBUG` variable with `False`.

# Run:
Start `mongod`, then when you in project dir with actived environment just type in terminal

`python web.py`

![builtin_run](http://i.imgur.com/dkEL5aS.png?2)

or

`gunicorn web:app`

![gunicorn_run](http://i.imgur.com/rCp0g25.png?2)

