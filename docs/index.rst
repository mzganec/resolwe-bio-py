
.. _index:

======================
Resolwe SDK for Python
======================

Resolwe SDK for Python supports interaction with Resolwe_ server
and its extension `Resolwe Bioinformatics`_. You can use it to upload
and inspect biomedical data sets, contribute annotations, run
analysis, and write pipelines.

.. _Resolwe Bioinformatics: https://github.com/genialis/resolwe-bio
.. _Resolwe: https://github.com/genialis/resolwe

Install
=======

Install from PyPI::

  pip install resdk

.. warning::

   If you use macOS, be aware that the version of `Python shipped with the
   system doesn't support TLSv1.2`_, which is required for connecting to
   any Resolwe server (and probably others). To solve the issue,
   install the latest version of Python 2.7 or Python 3 `via official
   installer from Python.org`_ or `with Homebrew`_.

.. _`Python shipped with the system doesn't support TLSv1.2`:
    http://pyfound.blogspot.si/2017/01/time-to-upgrade-your-python-tls-v12.html
.. _`via official installer from Python.org`:
    https://www.python.org/downloads/mac-osx/
.. _`with Homebrew`:
    http://docs.python-guide.org/en/latest/starting/install/osx/

If you would like to contribute to the SDK code base, follow the
:ref:`installation steps for developers <contributing>`.

Usage example
=============

We will download the aligned reads and the corresponding index from
the server:

.. literalinclude:: files/usage.py
   :lines: 1-13

Both files (BAM and BAI) have downloaded to the working directory.
Check them out. To learn more about the Resolwe SDK continue with
:ref:`tutorial`.

If you have problems connecting to our server, please contact us at
info@genialis.com.

Documentation
=============

.. toctree::
   :maxdepth: 2

   start
   tutorials
   ref
   contributing
