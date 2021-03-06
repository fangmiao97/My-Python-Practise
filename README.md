# FM's Python Practise
author: FANG Miao

 ## context

this is my Python practise project, not just something about basic variables and functions, but even more things also, like virtual environment...

## venv vs. virtualenv

* [comparison](https://virtualenv.pypa.io/en/latest/)

### venv

* build an virtual environment 

  `py3 -m venv venvname`

  venvname can be anything you want, but *.venv* commonly be used. I use *.venv* and *myenv* in this project, see in `FMPyProjects\venv-learn`

* active virtual env

  `.venv\Scripts\activate`

  using `activate` script in the venv(venvname) folder, then the terminal could be like,

  ![](https://pic.downk.cc/item/5f1e710514195aa594a9457f.jpg)

  pip install some specific libs in this environment, which will not impact other environment. choose interpreter in this environment to run some specific source code, like some libs just install in this env and other env cannot use.

  ![](https://pic.downk.cc/item/5f1e71ea14195aa594a9b91e.jpg)

* deactivate

  `deactivate` type this command will deactivate this env, but not delete it. if you want to delete some env, just delete the env folder but make sure that you are not using it.

### virtualenv

* install virtualenv

  `pip install --user virtialenv`

* build env

  `py -m virtualenv myenv`

  `cd myenv`

  `.\Scripts\activate // activate this env`

  deactivate same as the former one

  #### [virtualenvwrapper](https://pypi.org/project/virtualenvwrapper/)

  virtualenvwrapper is a set of extensions to [virtualenv](http://pypi.python.org/pypi/virtualenv) tool. Wrappers for creating, copying and deleting environments, including user-configurable hooks.

  there is a sad thing that I tried to install `virtualenvwrapper-win` and set the path `WORKON_HOME == ****` in the system already, but no response appear after I type command `workon` and `mkvirtualenv` *sigh*

  and I tried to install *virtualenvwrapper-powershell*, and its least version is 2012, obviously it's outdated. the setup.py in it is coded by python2, so some syntax error will appear. If you really want to it, no bother to switch to python2 : )

  ![](https://pic.downk.cc/item/5f1f8b0614195aa594645902.jpg)

  then I tried install *virtualenvwrapper-win* again, please use pip uninstall to delete some packages. If there are some error, please try to install those packages **in the admin mode.**

  set the system path var

  ![](https://pic.downk.cc/item/5f1f987514195aa5946e0fa7.jpg)

  ![](https://pic.downk.cc/item/5f1f989a14195aa5946e2804.jpg)

  ![](https://pic.downk.cc/item/5f1f990314195aa5946e6ab7.jpg)

```python
rmvirtualenv venv # remove env 
lsvirtualenv   # list all envs
cdvirtualenv    
cdsitepackages   
lssitepackages
```

