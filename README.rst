Instalation
===========
* Download this folder

``cd ``

``git clone git@github.com:bsuttor/python-tools.git``

``cd python-tools``

* Copy default.cfg for download eggs in local, and change path into default.cfg

``cp default.cfg ~/.buildout/default.cfg``

* Start bootstrap and buildout

``python bootstrap.py``

``bin/buildout -N``

* Add this line on .bashrc file :

``export PATH=~/python-tools/bin:$PATH``

