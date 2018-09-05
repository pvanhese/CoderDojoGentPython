.. include:: /global.rst

Installatie
===========

.. include:: <isonum.txt>

Installatie van Python
----------------------

Windows
~~~~~~~

https://www.python.org/downloads/windows/

Kies Python 3.7.0 64-bit |rarr| Download `Windows x86-64 executable installer`_.

In de installer, vink "Add Python 3.7 to PATH" aan.

.. admonition:: Test

   Open een Windows commando-venster met :kbd:`Win-R, cmd`, en check
   de Python-versie:

   .. code-block:: doscon

      > python -V
      Python 3.7.0


Meer uitleg is te vinden in `Installatie-instructies [Installatie Python.docx]`_.


.. _Windows x86-64 executable installer: https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe

.. _Installatie-instructies [Installatie Python.docx]: https://docs.google.com/document/d/1XaxzWhyDiMx94hDAjPL9FMIXcfV5nve-kAT4ARv0Obc



Installatie van pygame
----------------------

Windows
~~~~~~~

Maak een virtuele omgeving aan:

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

Installeer pygame:

.. code-block:: doscon

   (venv37) CoderDojo> pip install -U pygame


.. admonition:: Test

   .. code-block:: doscon

      (venv37) CoderDojo> python -m pygame.examples.aliens


Meer uitleg is te vinden in `Pygame Installation`_.

.. _Pygame Installation: https://www.pygame.org/wiki/GettingStarted



Installatie van IPython
-----------------------

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




.. IDLE
   ----

   Windows
   ~~~~~~~

   Open IDLE vanuit het Start-menu: "IDLE (Python 3.7 64 bit)".
   Dit toont de "Python 3.7.0 Shell".




Installatie van Kivy
--------------------

Windows
~~~~~~~

.. code-block:: doscon

   (venv37) CoderDojo> python -m pip install --upgrade pip wheel setuptools
   (venv37) CoderDojo> python -m pip install docutils pygments pypiwin32 kivy.deps.sdl2 kivy.deps.glew
   (venv37) CoderDojo> python -m pip install kivy.deps.gstreamer
   (venv37) CoderDojo> python -m pip install kivy


.. admonition:: Test

   .. code-block:: doscon

      (venv37) CoderDojo> ipython

   ::

      Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:59:51) [MSC v.1914 64 bit (AMD64)]
      Type 'copyright', 'credits' or 'license' for more information
      IPython 6.5.0 -- An enhanced Interactive Python. Type '?' for help.

      In [1]: import kivy
      Purge log fired. Analysing...
      Purge finished!
      [INFO   ] [Logger      ] Record log in C:\Users\P\.kivy\logs\kivy_18-08-17_0.txt
      [INFO   ] [Kivy        ] v1.10.1
      [INFO   ] [Python      ] v3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:59:51) [MSC v.1914 64 bit (AMD64)]


Meer uitleg is te vinden in `Kivy Installation on Windows`_.

.. _Kivy Installation on Windows: https://kivy.org/docs/installation/installation-windows.html#install-win-dist





