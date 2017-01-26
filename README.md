# Tor hidden for heroku
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
For opencart 
in root directory need hidden_service and tor folder
also torrc file needed in tor folder
```
mkdir hidden_service
mkdir tor
> tor/torrc
```
