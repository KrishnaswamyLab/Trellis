Implementation of Trellis
=========================
**Trellis tree-based analysis reveals stromal regulation of patient-derived organoid drug responses**

This library runs code associated with the Trellis paper which is now published in **Cell** and accessible  `here <https://www.sciencedirect.com/science/article/pii/S0092867423012205>`_.
A short how-to tutorial on Trellis is available `here <https://github.com/MariaRamosZ/Trellis_how_to/>`_, with associated notebook hosted on Kaggle `here <https://www.kaggle.com/code/mariaramosz/trellis>`_.
Code to reproduce the figures in the paper can be found on the `TapeLab's github repo
<https://github.com/TAPE-Lab/Ramos-et-al-Trellis>`_. Note that an earlier version of `MultiscaleEMD <https://github.com/atong01/MultiscaleEMD/>`_ was used to run these experiments. Installing this version can be accomplished by downloading the source at `this commit <https://github.com/atong01/MultiscaleEMD/tree/35f91c1aa4a209638d5884ea32afba64fe6a4960>`_ and installing with :code:`pip install -e .` from the :code:`MultiscaleEMD` directory.

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

Trellis is available in `pypi`. Install by running the following:

.. code-block:: bash

    pip install MultiscaleEMD

This code was tested with python 3.7-3.10. Issues can be filed directly on the `MultiscaleEMD <https://github.com/atong01/MultiscaleEMD/>`_ project.

Data
----
All mass cytometry files are available on `Cytobank <https://community.cytobank.org/cytobank/projects/1461>`_.

Compiled TOBis mass cytometry PDO-CAF dataframe is available on `Mendely <https://data.mendeley.com/datasets/hc8gxwks3p>`_.

References
----------

    @article{Ramos Zapatero2022.10.19.512668,
    	author = {Maria {Ramos Zapatero} and Alexander Tong and James W. Opzoomer and Rhianna O'Sullivan and Ferran {Cardoso Rodriguez} and Jahangir Sufi and Petra Vlckova and Callum Nattress and Xiao Qin and Jeroen Claus and Daniel Hochhauser and Smita Krishnaswamy and Christopher J. Tape},
    	journal = {Cell},
    	number = {25},
    	pages = {5606-5619.e24},
    	title = {Trellis tree-based analysis reveals stromal regulation of patient-derived organoid drug responses},
    	volume = {186},
    	year = {2023}
    }
