.. contents:: Table of Contents
   :depth: 2

tangrama.base.buildout
************************

Overview
--------

This is the base buildout for projects.

Requirements
------------

    - Python >=2.4 (http://www.python.org/download/releases)
    - Plone >=3.x (http://plone.org/products/plone)
    
Installation
------------
    
To enable this product,on a buildout based installation:

    1. Make clone a buildout::

        $ git clone git@bitbucket.org:simplesconsultoria/sample.git

    3. Add in your buildout the **extends**::
        
        [buildout]
        ...

        extends = https://raw.github.com/simplesconsultoria/tangrama.base.buildout/master/tangrama.cfg

        ...

    4. Modify and custom your buildout.cfg if necessary adding or removing parameters, eg::

        ...

        eggs += my.package
            
        [instance]
        zodb-cache-size = 15000

        ...

    5. Run::

        $ python bootstrap.py
        $ ./bin/buildout -Nv -t 30


Credits
-------

    * Simples Consultoria (products at simplesconsultoria dot com dot br) - 
      Implementation
