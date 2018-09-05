.. include:: /global.rst

Windows
=======

Installatie-instructies voor Python onder Windows.


Python
------

Download en gebruik de `Windows x86-64 executable installer`_
voor Python 3.7.0 64-bit.

.. _Windows x86-64 executable installer: https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe

.. https://www.python.org/downloads/windows/

In de installer, vink "Add Python 3.7 to PATH" aan.

.. admonition:: Test

   Open een Windows commando-venster met :kbd:`Win-R, cmd`, en controlleer
   de Python-versie:

   .. code-block:: doscon

      > python -V
      Python 3.7.0

.. admonition:: Test

   Open IDLE vanuit het Start-menu: "IDLE (Python 3.7 64 bit)".
   Dit toont de "Python 3.7.0 Shell".


Meer uitleg is te vinden in `Installatie-instructies [Installatie Python.docx]`_.

.. _Installatie-instructies [Installatie Python.docx]: https://docs.google.com/document/d/1XaxzWhyDiMx94hDAjPL9FMIXcfV5nve-kAT4ARv0Obc



pygame
------

Maak een `virtuele omgeving <https://docs.python.org/3/library/venv.html>`_ aan:

.. code-block:: doscon

   > mkdir CoderDojo
   CoderDojo> cd CoderDojo
   CoderDojo> python -m venv venv37

Gebruik de aangemaakte virtuele omgeving:

.. code-block:: doscon

   CoderDojo> venv37\Scripts\activate
   (venv37) CoderDojo>

Update pip:

.. code-block:: doscon

   (venv37) CoderDojo> python -m pip install --upgrade pip

Installeer `pygame <https://www.pygame.org/>`_ m.b.v. pip:

.. code-block:: doscon

   (venv37) CoderDojo> pip install -U pygame


.. admonition:: Test

   .. code-block:: doscon

      (venv37) CoderDojo> python -m pygame.examples.aliens


Meer uitleg is te vinden in `Pygame Installation`_.

.. _Pygame Installation: https://www.pygame.org/wiki/GettingStarted



IPython
-------

Installeer `IPython <https://ipython.org/>`_ m.b.v. pip:

.. code-block:: doscon

   (venv37) CoderDojo> pip install ipython


.. admonition:: Test

   .. code-block:: doscon

      (venv37) CoderDojo> ipython -V
      6.5.0

      (venv37) CoderDojo> ipython

   ::

      Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:59:51) [MSC v.1914 64 bit (AMD64)]
      Type 'copyright', 'credits' or 'license' for more information
      IPython 6.5.0 -- An enhanced Interactive Python. Type '?' for help.

      In [1]: print("Hi!")
      Hi!

      In [2]: 2 + 2
      Out[2]: 4

      In [3]:

   Sluit IPython met :kbd:`Ctrl-D`.



Kivy
----

`Kivy <https://kivy.org/>`_ heb je enkel nodig voor de :ref:`extraoefeningen`.

Installeer Kivy m.b.v. pip:

.. code-block:: doscon

   (venv37) CoderDojo> python -m pip install --upgrade pip wheel setuptools
   (venv37) CoderDojo> python -m pip install docutils pygments pypiwin32 kivy.deps.sdl2 kivy.deps.glew
   (venv37) CoderDojo> python -m pip install kivy.deps.gstreamer
   (venv37) CoderDojo> python -m pip install kivy

.. admonition:: Test

   .. code-block:: doscon

      (venv37) CoderDojo> python

   ::

      Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:59:51) [MSC v.1914 64 bit (AMD64)] on win32
      Type "help", "copyright", "credits" or "license" for more information.
      >>> import kivy
      [INFO   ] [Logger      ] Record log in C:\Users\user\.kivy\logs\...txt
      [INFO   ] [Kivy        ] v1.10.1
      [INFO   ] [Python      ] v3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:59:51) [MSC v.1914 64 bit (AMD64)]



Meer uitleg is te vinden in `Kivy Installation on Windows`_.

.. _Kivy Installation on Windows: https://kivy.org/docs/installation/installation-windows.html#install-win-dist
