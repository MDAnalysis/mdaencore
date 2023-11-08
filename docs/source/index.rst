.. mdaencore documentation master file, created by
   sphinx-quickstart on Thu Mar 15 13:55:56 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to mdaencore's documentation!
=========================================================

.. toctree::
   :maxdepth: 1
   :caption: Contents:
   :hidden:

   getting_started
   api

The package contains implementations of similarity measures between protein
ensembles described in :footcite:p:`LindorffLarsen2009`. The implementation and examples
are described in :footcite:p:`Tiberti2015`.

The module includes facilities for handling ensembles and trajectories through
the :class:`Universe` class, performing clustering or dimensionality reduction
of the ensemble space, estimating multivariate probability distributions from
the input data, and more. ENCORE can be used to compare experimental and
simulation-derived ensembles, as well as estimate the convergence of
trajectories from time-dependent simulations.

ENCORE includes three different methods for calculations of similarity measures
between ensembles implemented in individual functions:

+ **Harmonic Ensemble Similarity** : :func:`~mdaencore.similarity.hes`
+ **Clustering Ensemble Similarity** : :func:`~mdaencore.similarity.ces`
+ **Dimensional Reduction Ensemble Similarity** : :func:`mdaencore.similarity.dres`

as well as two methods to evaluate the convergence of trajectories:

+ **Clustering based convergence evaluation** : :func:`mdaencore.similarity.ces_convergence`
+ **Dimensionality-reduction based convergence evaluation** : :func:`mdaencore.similarity.dres_convergence`

When using this module in published work please cite :footcite:p:`Tiberti2015`.

.. seealso::

   For higher level examples of how to use the software, see the `ENCORE section <https://userguide.mdanalysis.org/stable/examples/analysis/trajectory_similarity/clustering_ensemble_similarity.html>`_ of the MDAnalysis User Guide.
   Note that the user guide imports the ENCORE implementation in the core library, as the current version of MDAnalysis still has this functionality.
   To use these examples, import ``mdaencore`` rather than ``MDAnalysis.analysis.encore``.

The `mdaencore` MDAKit moves the functionality of integrated ENCORE module out of the MDAnalysis core library, thereby deprecating it in MDAnalysis release 2.7.0 with a planned removal in release 3.0.0.
The original authors for the MDAnalysis implementation of ENCORE are  Matteo Tiberti, Wouter Boomsma, Tone Bengtsen, as well as those listed in ``AUTHORS.md``.

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

References
----------

.. footbibliography::
