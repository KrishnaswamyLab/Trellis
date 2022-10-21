Implementation of Trellis
=========================

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

Data
----
All mass cytometry files are available on `Cytobank<https://community.cytobank.org/cytobank/projects/1461>`_

Compiled TOB\textit{is} mass cytometry PDO-CAF dataframe is available at: Ramos, Maria (2022), “Ramos Zapatero et. al (Cancer-Associated Fibroblasts Regulate Patient-Derived Organoid Drug Responses)”, Mendeley Data, V1, doi: 10.17632/hc8gxwks3p.1

References
----------

TODO: Reference BioArXiv
