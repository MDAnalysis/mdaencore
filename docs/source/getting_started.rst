Getting Started
===============

Installation
------------

`mdaencore` is currently only installable from source.
First download and navigate to the source code from GitHub with

.. code-block:: sh

	git clone --depth=1 https://github.com/MDAnalysis/mdaencore.git
	cd mdaencore

The packages is now installable with `pip`:

.. code-block:: sh

	pip install .

For full functionality of the :func:`mdaencore.fit_clusters` function, also install the `scikit-learn` package

.. code-block:: sh

	pip install scikit-learn