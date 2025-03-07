======
msm_we
======

.. image:: https://github.com/westpa/msm_we/actions/workflows/test.yml/badge.svg
        :target: https://github.com/westpa/msm_we/actions/workflows/test.yml

.. image:: https://github.com/jdrusso/msm_we/actions/workflows/main.yml/badge.svg
        :target: https://github.com/jdrusso/msm_we/actions/workflows/main.yml


Code for Markov state modeling of weighted ensemble trajectories.

* Authors: John Russo, Jeremy Copperman
* Free software: MIT license
* Documentation: https://jdrusso.github.io/msm_we/ .


Features
--------

* Compute a history-augmented Markov state model from WESTPA weighted ensemble data
* Estimate steady-state distributions
* Estimate flux profiles
* Estimate committors


Code development TODOs
-----
*  Provide option for user to override :code:`dimReduce()` in case they want to do something other than PCA/VAMP
*  Add TICA option to :code:`dimReduce()`
*  Add monkey-patching directly into :code:`msm_we` code.
   I.e., add a function like :code:`register_featurization(func)` which takes the featurization function as input and
   overloads :code:`msm_we.processCoordinates()` with it.
   Right now, this has to be done manually.


Credits
-------

This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
