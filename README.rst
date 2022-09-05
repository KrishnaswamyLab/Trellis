Pytorch Implementation of Trellis
=================================

This library runs code associated with the Trellis paper. Code to reproduce the
figures in the paper can be found on the `TapeLab's github repo
<https://github.com/TAPE-Lab/Ramos-et-al-Trellis>`_.

In brief, Trellis is a method to compare single-cell dataset distributions
under different treatment conditions while normalizing for multiple controls.
Paired Trellis implements a Kantorovich-Rubenstein distance with tree ground
distance allowing for a normalization step against a specified control per
treatment. 

.. image:: figures/abstract.png
    :alt: Trellis Graphical Abstract
    :height: 300



Installation
------------

Trellis is available in `pypi`. Install by running the following

.. code-block:: bash

    pip install MultiscaleEMD

This code was tested with python 3.7 and 3.8.

Basic Usage
-----------

See `notebooks/EB-Eval.ipynb` for an example on how to use Trellis on
a PCA embedding to get trajectories in the gene space.

References
----------

TODO: Reference BioArXiv
