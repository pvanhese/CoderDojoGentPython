.. include:: /global.rst

Mac OS X
========

Installatie-instructies voor Python onder Mac OS X.


Python
------

Download en gebruik de `macOS 64-bit installer`_ voor Python 3.7.0 64 bit.

.. _macOS 64-bit installer: https://www.python.org/ftp/python/3.7.0/python-3.7.0-macosx10.9.pkg

.. https://www.python.org/downloads/mac-osx/

.. admonition:: Test

   Open een terminal-venster met :kbd:`cmd + spatie, Terminal`, en controlleer
   de Python-versie:

   .. code-block:: bash

      ~ user$ python3 -V
      Python 3.7.0



pygame
------

Maak een `virtuele omgeving <https://docs.python.org/3/library/venv.html>`_ aan:

.. code-block:: bash

   ~ user$ mkdir CoderDojo
   ~ user$ cd CoderDojo
   CoderDojo user$ python3 -m venv venv37

Gebruik de aangemaakte virtuele omgeving:

.. code-block:: bash

   CoderDojo user$ source venv37/bin/activate
   (venv37) CoderDojo user$

Update pip:

.. code-block:: bash

   (venv37) CoderDojo user$ pip install --upgrade pip

Installeer `pygame <https://www.pygame.org/>`_ m.b.v. pip:

.. code-block:: bash

   (venv37) CoderDojo user$ pip install -U pygame


.. admonition:: Test

   .. code-block:: bash

      (venv37) CoderDojo user$ python -m pygame.examples.aliens


Meer uitleg is te vinden in `Pygame Installation`_.

.. _Pygame Installation: https://www.pygame.org/wiki/GettingStarted



IPython
-------

Installeer `IPython <https://ipython.org/>`_ m.b.v. pip:

.. code-block:: bash

   (venv37) CoderDojo user$ pip install ipython


.. admonition:: Test

   .. code-block:: bash

      (venv37) CoderDojo user$ ipython -V
      6.5.0

      (venv37) CoderDojo user$ ipython

   ::

      Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 26 2018, 23:26:24)
      Type 'copyright', 'credits' or 'license' for more information
      IPython 6.5.0 -- An enhanced Interactive Python. Type '?' for help.

      In [1]: print("Hi!")
      Hi!

      In [2]: 2 + 2
      Out[2]: 4

      In [3]:

   Sluit IPython met :kbd:`Ctrl-D, y`.



Kivy
----

`Kivy <https://kivy.org/>`_ heb je enkel nodig voor de :ref:`extraoefeningen`.

Installeer `Homebrew <https://brew.sh/>`_:

.. code-block:: bash

   ~ user$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Gebruik Homebrew voor de installatie van de bibliotheken die Kivy nodig heeft:

.. code-block:: bash

   ~ user$ brew install pkg-config sdl2 sdl2_image sdl2_ttf sdl2_mixer gstreamer

In je virtuele omgeving, installeer Cython en Kivy m.b.v. pip:

.. code-block:: bash

   ~ user$ cd CoderDojo
   CoderDojo user$ source venv37/bin/activate
   (venv37) CoderDojo user$ pip install -U Cython
   (venv37) CoderDojo user$ pip install kivy

.. admonition:: Test

   .. code-block:: bash

      (venv37) CoderDojo user$ python

   ::

      Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 26 2018, 23:26:24)
      [Clang 6.0 (clang-600.0.57)] on darwin
      Type "help", "copyright", "credits" or "license" for more information.
      >>> import kivy
      [INFO   ] [Logger      ] Record log in /Users/user/.kviy/logs/...txt
      [INFO   ] [Kivy        ] v1.10.1
      [INFO   ] [Python      ] v3.7.0 (v3.7.0:1bf9cc5093, Jun 26 2018, 23:26:24)
      [Clang 6.0 (clang-600.0.57)]

   Sluit met :kbd:`Ctrl-D`.


Meer uitleg is te vinden in `Kivy Installation on OS X`_.

.. _Kivy Installation on OS X: https://kivy.org/doc/stable/installation/installation-osx.html
