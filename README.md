# Toroku
Experimental Tor Hidden Service hosting on Heroku

How do you get these variables?
The easiest way is to:<br>

<span>
$ heroku run bash<br>
heroku$ mkdir hidden<br>
heroku$ echo "HiddenServiceDir /app/hidden/" > tmptorrc<br>
heroku$ echo "HiddenServicePort 80 127.0.0.1:8000" >> tmptorrc<br>
heroku$ tor -f tmptorrc<br>
heroku$ cat hidden/*<br>
heroku$ ^D<br>
</span>
