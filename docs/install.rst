How to install
****************************

.. toctree::

Using pip
---------

If you are using `pyenv <https://github.com/yyuu/pyenv>`_ or don't need special root access to install:

.. code:: console

	  $ pip install trepan2 # or trepan3k for Python 3.x


If you need root access you may insert `sudo` in front or become root:

.. code:: console

	  $ sudo pip install trepan2

or:

.. code:: console

	  $ su root
	  # pip install trepan

Using easy_install
------------------

Basically the same as using *pip*, but change "pip install" to "easy_install":

.. code:: console

	  $ easy_install trepan  # or trepan3k

.. code:: console

	  $ git clone https://github.com/rocky/python2-trepan.git
	  $ cd python-trepan
	  $ make check-short # to run tests
	  $ make install # if pythonbrew or you don't need root access
	  $ sudo make install # if pythonbrew or you do need root access

Above I used GNU "make" to run and install. However this just calls `python setup.py` to do the right thing. So if you are more familiar with `setup.py` you can use that directly. For example:

.. code:: console

	  $ ./setup.py test
	  $ ./setup.py install
