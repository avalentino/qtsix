=====
QtSix
=====

.. image:: https://img.shields.io/pypi/dm/qtsix.svg
    :target: https://pypi.python.org/pypi//qtsix/
    :alt: Downloads

.. image:: https://img.shields.io/pypi/v/qtsix.svg
    :target: https://pypi.python.org/pypi/qtsix/
    :alt: Latest Version

.. image:: https://img.shields.io/pypi/pyversions/qtsix.svg
    :target: https://pypi.python.org/pypi/qtsix/
    :alt: Supported Python versions

.. image:: https://img.shields.io/pypi/l/qtsix.svg
    :target: https://pypi.python.org/pypi/qtsix/
    :alt: License


About
=====

*QtSix* provides a compatibility layer that allows to write Python
applications that work with different Qt_ bindings: PyQt5_, PyQt4_ or
PySide_.

An application that used *QtSix* can work correctly if **any** of the
supported Qt_ bindings is installed on the system.
*QtSix* automatically detects available bindings and uses them
transparently.

If more than one Qt_ binding is present on the system then it is selected
the first one available in the following order: PyQt5_, PyQt4_, PySide_.

Of course *QtSix* supports both `Python 2`_ and `Python 3`_.


The API
=======

The reference API and the reference package layout used by *QtSix* is
the one provided by PyQt5_.

An application written for PyQt5_ is expected to work correctly if
all imports form PyQt5_ are replaced with imports from *QtSix*.

Applications written for PyQt4_ or PySide_ should be ported to the PyQt5_
API in order to be able to use *QtSix*.

Since *QtSix* is meant to be a compatibility layer it only provides
PyQt5_ features that are also present in at least one of the other Qt_
bindings.


Installation
============

*QtSix* can be installed using pip_::

    $ pip install qtsix

or using the `setup.py` script included in the package::

    $ python setup.py install

.. note::

    The desired Qt_ bindings should be installed separately.
    The installation of *QtSix* does not automatically trigger the
    installation of any of the supported Qt_ bindings.


Links
=====

* Home page: https://github.com/avalentino/qtsix
* Changelog: https://github.com/avalentino/qtsix/blob/master/NEWS.rst
* Issue tracker: https://github.com/avalentino/qtsix/issues
* Download: https://github.com/avalentino/qtsix/releases
* PyPi: https://pypi.python.org/pypi/qtsix


Similar projects
================

* PyQtX: https://github.com/kpj/PyQtX
* pyqode.qt: https://github.com/pyQode/pyqode.qt
* qt_backport: https://github.com/rwarren/qt_backport
* pyqt4topyqt5: https://github.com/rferrazz/pyqt4topyqt5
* q45aide: https://github.com/tallforasmurf/q45aide
* pyface: https://github.com/enthought/pyface


License
=======

The *QtSix* package is provided under the terms of the new `BSD license`_.


.. _Qt: http://qt-project.org
.. _PyQt5: http://www.riverbankcomputing.com/software/pyqt/intro
.. _PyQt4: http://www.riverbankcomputing.com/software/pyqt/intro
.. _PySide: http://pyside.org
.. _`Python 2`: https://docs.python.org/2/
.. _`Python 3`: https://docs.python.org/3/
.. _pip: https://pip.pypa.io
.. _`BSD license`: http://opensource.org/licenses/BSD-3-Clause

