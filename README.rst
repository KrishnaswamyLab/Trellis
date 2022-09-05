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
    \textbf{Trellis.} \textbf{a)} Single-cells from control and variable
    conditions are distributed through a tree comprising fixed binary
    `branches' that supervene upon randomized $k$-means clustering nodes,
    ending in `leaves'. Fixed branches weigh hierarchical gating strategies
    while nodes and leaves still leverage latent parameters. In each node of
    the tree variables are subtracted from paired controls to create a
    multi-scaled differential matrix (based on a kantorovich-rubinstein norm)
    that scales to thousands of conditions. \textbf{b)} Single-cell density
    PHATEs of PDO 21 treated with DMSO or SN-38 (irinotecan). SN-38 results
    in cell-cycle exit (IdU$^{-}$, pHH3$^{-}$, and pRB$^{-}$) and induction
    of apoptosis (cPARP$^{+}$). \textbf{c)} Trellis hierarchy for single-cell
    PDO drug responses leveraging fixed cell-state branches and randomized
    PTM and DNA-damage parameters. Trellis scores are calculated per PDO by
    comparing untreated controls to drugs for both mono-cultures and
    co-cultures. \textbf{d)} Sankey diagram showing data from {b)}
    distributing through the Trellis layout in c) (terminal leaves not
    shown).


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
