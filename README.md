## Rompy instalation

```
pip3 install virtualenv
pip3 install virtualenvwrapper
```

Add the following lines on yours shell config file (.bashrc, .zshrc, etc)

```
export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3.7  # or ../python2.7 or whatever
export WORKON_HOME=$HOME/.virtualenvs
export PROJECT_HOME=$HOME/Devel
source /usr/local/bin/virtualenvwrapper.sh
```

Open new bash session

Now we can create new virtualenvs!

```
mkvirtualenv --no-site-packages --python=python3.7 rom-3.7
```

And the new virtualenv is created!

Note: Is important to have pythonX binary at __/usr/local/bin__ (installed)

To activate the virtualenv we have to type:
```
workon [my_virtualenv_name]
```

Now we can see something like __(rom-3.7) [ 10:59AM ]  [ user@AR0FVFWR13KHV2J:~/ ]__

Go to the project root and run
```
pip install -r requirements.txt
```

Refs:
https://virtualenvwrapper.readthedocs.io/en/latest/install.html#python-versions
