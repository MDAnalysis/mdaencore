Getting Started
===============

Install the :mod:`mdaencore` package by any of the methods described below:

Installation
------------

From conda-forge
................

Install `mdaencore from the conda-forge channel`_ 
by first adding ``conda-forge`` to your channels with:

.. code-block:: sh

   conda config --add channels conda-forge
   conda config --set channel_priority strict

Once the ``conda-forge`` channel has been enabled, ``mdaencore`` can be installed with :program:`conda`:

.. code-block:: sh

   conda install mdaencore

or with :program:`mamba` (if you have it installed):

.. code-block:: sh

   mamba install mdaencore


From the Python Package Index PyPi
..................................

Install `mdaencore from PyPi`_ with :program:`pip`:

.. code-block:: sh

   pip install mdaencore


From source
...........

:mod:`mdaencore` can also be installed from `source`_.
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

Testing your installation
-------------------------
Install ``pytest`` and the ``mdanalysistests`` package (either with :program:`conda` or :program:`pip`).
Run the tests with

.. code-block:: sh

   pytest -v --pyargs mdaencore.tests

You should see the tests running and finishing with no failures. It may look similar to the following::

   ============================= 57 passed, 2 xpassed, 11 warnings in 24.48s ==============================

(The exact numbers may differ but there should be no failed tests.)


.. _`mdaencore from the conda-forge channel`: https://anaconda.org/conda-forge/mdaencore
.. _`mdaencore from PyPi`: https://pypi.org/project/mdaencore/
.. _source: https://github.com/MDAnalysis/mdaencore/
