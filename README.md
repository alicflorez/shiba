Shiba
=====

shiba 1.0

Released: 11-Sep-2014

Introduction
--------------

Shiba is a Python package that provides interfaces to PriceMinister Web services. Currently, all features work
with Python 2.6 and 2.7.

Shiba supports all the Web services introduced by the PriceMinister developper blog.

The goal of Shiba is to provide PriceMinister active buyers/sellers an easy way to do their daily tasks for a good management
of their account.

Installation
______________

Install via [pip](http://pip-installer.org/):

::
	$ pip install shiba

Install from source:

::
	$ git clone git://github.com/shibaAPI/shiba.git
	$ cd shiba
	$ python setup.py install


Quick starting with Shiba
-------------------------
Import the `shibaconnection` module first, then the module(s) you wish to work with.

Instance the ShibaConnection class with your credentials, then instance the other modules with the newly created ShibaConnection instance.

You're good to go!

Example:

::

	from Shiba.shibaconnection import ShibaConnection
	from Shiba.salesmanagement import SalesManagement

	connection = ShibaConnection("mylogin", "mytoken")
	sales = SalesManagement(connection)
	newsales = sales.get_new_sales()


Documentation
--------------
Documentation is available [here](http://ShibaAPI.github.io/shiba/) on **GitHub pages**.
Extra documentation from the [PriceMinister developper blog](https://developer.priceminister.com/blog/) might be useful.

Feel free to comment, report bugs, or even contribute!

*Thank you!*