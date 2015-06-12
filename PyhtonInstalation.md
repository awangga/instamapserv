#How To Install Python 2.7.

# Introduction #

Installing Python 2.7 on RHEL 6 from repo
http://people.redhat.com/bkabrda/python27-rhel-6/

# Details #

```
#!/bin/bash

wget http://people.redhat.com/bkabrda/python27-rhel-6/python27-runtime-1.1-15.el6.x86_64.rpm

rpm -ivh python27-runtime-1.1-15.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-libs-2.7.5-10.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-2.7.5-10.el6.x86_64.rpm


rpm -ivh python27-python-libs-2.7.5-10.el6.x86_64.rpm python27-python-2.7.5-10.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-babel-0.9.6-7.el6.noarch.rpm

rpm -ivh python27-python-babel-0.9.6-7.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-markupsafe-0.11-11.el6.x86_64.rpm

rpm -ivh python27-python-markupsafe-0.11-11.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-jinja2-2.6-9.el6.noarch.rpm

rpm -ivh python27-python-jinja2-2.6-9.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-setuptools-0.9.8-1.el6.noarch.rpm

rpm -ivh python27-python-setuptools-0.9.8-1.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-nose-1.3.0-1.el6.noarch.rpm

rpm -ivh python27-python-nose-1.3.0-1.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-simplejson-3.2.0-1.el6.x86_64.rpm

rpm -ivh python27-python-simplejson-3.2.0-1.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-docutils-0.11-1.el6.noarch.rpm	

rpm -ivh python27-python-docutils-0.11-1.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-pygments-1.5-2.el6.noarch.rpm

rpm -ivh python27-python-pygments-1.5-2.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-sphinx-1.1.3-7.el6.noarch.rpm

rpm -ivh python27-python-sphinx-1.1.3-7.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-sqlalchemy-0.7.9-3.el6.x86_64.rpm

rpm -ivh python27-python-sqlalchemy-0.7.9-3.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-devel-2.7.5-10.el6.x86_64.rpm

rpm -ivh python27-python-devel-2.7.5-10.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-virtualenv-1.10.1-2.el6.noarch.rpm

rpm -ivh python27-python-virtualenv-1.10.1-2.el6.noarch.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-python-werkzeug-0.8.3-5.el6.noarch.rpm

rpm -ivh python27-python-werkzeug-0.8.3-5.el6.noarch.rpm


http://people.redhat.com/bkabrda/python27-rhel-6/python27-1.1-15.el6.x86_64.rpm

rpm -ivh python27-1.1-15.el6.x86_64.rpm

http://people.redhat.com/bkabrda/python27-rhel-6/python27-MySQL-python-1.2.3-10.el6.x86_64.rpm

rpm -ivh python27-MySQL-python-1.2.3-10.el6.x86_64.rpm

scl -l

scl enable python27 bash

python -V



```