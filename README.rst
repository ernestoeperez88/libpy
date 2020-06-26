``libpy``
=========

.. image:: https://github.com/quantopian/libpy/workflows/CI/badge.svg
    :alt: GitHub Actions status
    :target: https://github.com/quantopian/libpy/actions?query=workflow%3ACI+branch%3Amaster

.. image:: https://badge.fury.io/py/libpy.svg
    :target: https://badge.fury.io/py/libpy

``libpy`` is a lbrary to help you write amazing Python extensions in C++. ``libpy``makes it easy to expose C++ code to Python. It lets you automatically wrap functions and classes. It is designed for high performance and safety, so using libpy should be both faster and safer than using the C api directly.

`Full documentation <https://quantopian.github.io/libpy/>`_

Requirements
------------

libpy supports:

- macOS/Linux
- Python >=3.5

libpy requires:

- gcc>=8 or clang>=10
- numpy>=1.11.3

libpy also depends on:

- pcre
- google sparsehash

To install these dependencies:

ubuntu
~~~~~~

.. code-block:: bash

    $ sudo apt install libpcre2-dev libsparsehash-dev

macOS
~~~~~

.. code-block:: bash

    $ brew install pcre2 google-sparsehash

Install
-------

To install for development:

.. code-block:: bash

   $ make

Otherwise, ``pip install libpy``, making sure ``CC`` and ``CXX`` environment variables are set to the the right compiler.


Tests
-----

To run the unit tests, invoke:

.. code-block:: bash

   $ make test
