:title: Python para no pythonistas
:data-transition-duration: 1
:css: psm.css

----

:id: title

Python para no pythonistas
===========================

.. image:: img/AHJ1PC1e.png
	:height: 200px
	:width: 200px

----

:id: wololo-1

WOLOLO
======

- https://www.youtube.com/watch?v=3tBqdKGiqnI


----

:id: wololo-2

- Python Vigo: https://python-vigo.es
- VigoTech: https://vigotech.org

----

:id: introduction-1

Python
======

- First release in 1991 by Guido.
- Code readability
- Open source
- Comunity
- Diversity_.
- PSF. https://www.python.org/psf/
- Fun to use (Monty Python)

.. _Diversity: https://www.python.org/community/diversity/

----

:id: introduction-2

Introduction
============

- Python (https://www.python.org/)
- Official `documentation <https://docs.python.org/3/library/>`_.
- `Python Enhancement Proposals (PEP's). PEP8, PEP20 <https://www.python.org/dev/peps/>`_.
- Versatilidad del lenguaje

----

:id: introduction-3

Introduction
============

Grandes empresas que usan Python:

- Wikipedia
- Google,Yahoo!
- CERN, NASA,Facebook,
- Amazon, Instagram, Spotify.

----

:id: running-python

Running Python
===============

Install&Execute Python
----------------------
- `Official <https://www.python.org/downloads/>`_.
- `Pyenv <https://github.com/pyenv/pyenv>`_.
- Homebrew

	.. code:: python

		python --version
		python

----

Environments
============

- `Virtualenvs <https://docs.python.org/3/library/venv.html>`_.
- Never "sudo"

	.. code:: python

		python3 -m venv .venv
		source .venv/bin/activate

----

Package manager
===============

- `Pip <https://packaging.python.org/tutorials/installing-packages/#ensure-you-can-run-pip-from-the-command-line>`_.

	.. code:: python

		pip install <package>

----

Package manager
===============

- pipsi = pip script installer
- pipenv

----

:id: tools-1

Tools:
======

- `Flake8 <http://flake8.pycqa.org/en/latest/>`_
- `PEP8 <https://legacy.python.org/dev/peps/pep-0008/>`_

`BTW <https://legacy.python.org/dev/peps/pep-0008/#a-foolish-consistency-is-the-hobgoblin-of-little-minds>`_:

``In particular: do not break backwards compatibility just to comply with this PEP!``

----

:id: tools-2

Tools:
======

- `Isort <https://github.com/timothycrosley/isort>`_
- `How? <https://github.com/timothycrosley/isort#how-does-isort-work>`_

----

:id: tools-3

Tools:
======

- `Tox <https://tox.readthedocs.io/en/latest/>`_

.. code::

	[tox]
	envlist = py37,flake8,isort
	skipsdist = True

	[testenv:flake8]
	basepython=python3.7
	deps=flake8
	commands=flake8 .

	[testenv:isort]
	basepython=python3.7
	deps=isort
	commands=isort --check-only

----

:id: tools-4

Tools:
======

- `Black - The uncompromising Python code formatter <https://github.com/ambv/black>`_

*Beta!*

----

Flake8 & Isort
==============

``git@github.com:alexhermida/workshops.git``

	- lights_blink_remote.py
	- lights_on_subscriber.py

----

:id: pythonic-1

Idiomatic Python & Style
------------------------

- Years of developers experience
- Tuned to the CPython runtime
- Easily to read and understood by Python developers
- Often Cleaner and simpler
- Easy for other contributors to join
- Easy onboard Python developers

----

:id: pythonic-2

Idiomatic Python & Style
------------------------

- `String formatting <https://realpython.com/python-string-formatting/#2-new-style-string-formatting-strformat>`_
- `Loops <https://docs.python-guide.org/writing/style/#filtering-a-list>`_

----

:id: testing

Libraries
---------

	- `Unittest <https://docs.python.org/3/library/unittest.html> `_
	- `Pytest <https://docs.pytest.org/en/latest/>`_

----

:id: resources-links

Resources:
==========

* https://docs.python.org/3/reference/

----


Thanks!
=======

.. image:: img/AHJ1PC1e.png
	:height: 200px
	:width: 200px

@alexhermida
