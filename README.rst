Plone developer tools
=====================
.. contents::

After Ubuntu installation
-------------------------
Add some packages::

    sudo apt-get install python-dev build-essential libssl-dev libxml2-dev libxslt1-dev libbz2-dev libjpeg62-dev libreadline-gplv2-dev wv poppler-utils
    sudo apt-get install git subversion vim python-virtualenv

Add pythons
-----------
I use this repo https://github.com/collective/buildout.python for installing python. 
I develop with buildout and virtualenv.::

  cd
  git clone git://github.com/collective/buildout.python.git python

After, modify buildout.cfg and choose which pythons you needed. And launch buildout::

  cd
  cd python
  virtualenv tmpython
  tmpython/bin/python bootstrap.py
  bin/buildout -Nt 4

Finaly add this line on ~/.bashrc file::
  
  export PATH=~/python/bin:$PATH


Add developper tools
--------------------
Download this repo::

  cd
  git clone git@github.com:bsuttor/python-tools.git
  cd python-tools

Copy default.cfg for download eggs in local, and change path into default.cfg::

  cp default.cfg ~/.buildout/default.cfg

Start bootstrap and buildout::

  python bootstrap.py
  bin/buildout -Nt 4

Add this line on .bashrc file :::

  export PATH=~/python-tools/bin:$PATH

