# Toroku
Experimental Tor Hidden Service hosting on Heroku

How do you get these variables?
The easiest way is to:

```
$ heroku run bash
heroku$ mkdir hidden
heroku$ echo "HiddenServiceDir /app/hidden/" > tmptorrc
heroku$ echo "HiddenServicePort 80 127.0.0.1:8000" >> tmptorrc
heroku$ tor -f tmptorrc
heroku$ cat hidden/*
heroku$ ^D
```
