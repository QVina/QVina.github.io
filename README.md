
<h1>Welcome to QuickVina!</h1>

Quick Vina 2
-------------
Quick Vina 2 is a fast and accurate molecular docking tool, attained at accurately accelerating AutoDock Vina. It was tested against 195 protein–ligand complexes that compose the core set of the 2014 release of the PDBbind using default exhaustiveness level of 8, QVina 2 successfully attained up to 20.49-fold acceleration over Vina. The Pearson’s correlation coefficient between Vina’s QVina 2’s binding energy was 0.967 for the first predicted mode and 0.911 for the sum of all predicted modes.

It is also witnessed that QVina 2 is more accurate than GOLD 5.2 and is only slightly less accurate than Dock 6.6. This shows that QVina 2 has paved the way for some high-throughput and sufficiently accurate virtual screening of molecular libraries. This in turn brings great value to the fragment-based computer-aided drug design.


![Example](https://github.com/QVina/QVina.github.io/blob/master/fig7.png)



To cite QuickVina 2 please cite:

__"Fast, Accurate, and Reliable Molecular Docking with QuickVina 2"__
Amr Alhossary, Stephanus Daniel Handoko, Yuguang Mu, and Chee-Keong Kwoh. Bioinformatics (2015) 31 (13): 2214-2216. [DOI:10.1093/bioinformatics/btv082](https://doi.org/10.1093/bioinformatics/btv082)



QuickVina-W
--------------

Virtual Screening” is a common step of in silico drug design, where researchers screen a large library of small molecules (ligands) for interesting hits, in a process known as “Docking”. However, docking is a computationally intensive and time-consuming process, usually restricted to small size binding sites (pockets) and small number of interacting residues. When the target site is not known (blind docking), researchers split the docking box into multiple boxes, or repeat the search several times using different seeds, and then merge the results manually. Otherwise, the search time becomes impractically long. 

In this research, we studied the relation between the search progression and Average Sum of Proximity relative Frequencies (ASoF) of searching threads, which is closely related to the search speed and accuracy. A new inter-process spatio-temporal integration method is employed in Quick Vina 2, resulting in a new docking tool, QuickVina-W, a suitable tool for “blind docking”, (not limited in search space size or number of residues). QuickVina-W is faster than Quick Vina 2, yet better than AutoDock Vina. It should allow screening huge ligand libraries virtually, in practically short time and with high accuracy without the need to define a target pocket beforehand.


To cite QuickVina-W please cite:

__"Protein-Ligand Blind Docking Using QuickVina-W With Inter-Process Spatio-Temporal Integration"__
Nafisa M. Hassan, Amr A. Alhossary, Yuguang Mu & Chee-Keong Kwoh. Nature Scientific Reports 7(1) (2017). [DOI:10.1038/s41598-017-15571-7](http://dx.doi.org/10.1038/s41598-017-15571-7)

### important note:
* If you Don't know the Docking site, then QuickVina-W is your choice with the ability to dock a _WIDE_ search box.
* However if you _know_ the target search box, we recommend that you use QuickVina 2.


Having any inquiries, please contact us<br>
<a href= "mailto:aalhossary@pmail.ntu.edu.sg"> Amr Alhossary </a> <br>
<a href= "mailto:nafisa.mohamed@ntu.edu.sg"> Nafisa Mohamed </a> <br>


Your feedback is highly appreciated. We hope to hear from you soon!


