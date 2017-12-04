
<h1>Welcome to QuickVina!</h1>

Quick Vina 2
-------------
Quick Vina 2 is a fast and accurate molecular docking tool, attained at accurately accelerating AutoDock Vina. It was tested against 195 protein–ligand complexes that compose the core set of the 2014 release of the PDBbind using default exhaustiveness level of 8, QVina 2 successfully attained up to 20.49-fold acceleration over Vina. The Pearson’s correlation coefficient between Vina’s QVina 2’s binding energy was 0.967 for the first predicted mode and 0.911 for the sum of all predicted modes.

The following figure shows the binding energies of the first predicted modes in QVina 1 and 2 on the vertical axis, against their corresponding modes in original Vina on the horizontal axis. The binding Energies of QVina 2 are almost identical to those of Vina. The Pearson’s correlation coefficient (r) for the two pairs was 0.967 between Vina and QVina 2, while it was only 0.780 between Vina and QVina 1. The same observation was also observed for the sums of all predicted modes where the respective values were 0.912 and 0.637

![Binding energy](https://github.com/QVina/QVina.github.io/raw/master/qvina2 fig 3 binding energy.png)

Next, the following figure shows that 70% of first predicted modes from QVina 2 are equal to or better than Vina predicted modes, in terms of Binding Energy. Even the remaining 30% have an average Energy difference as small as 0.58 Kcal/mol. On the contrary, the ratio is almost reversed for QVina 1: Only 37% are equal to or better than the Original Vina, and the remaining 63% have an average E difference as far as 1.56 Kcal/mol. Percentage of predictions with the same Binding Energies is shown in the middle part, while those with better Energy (more negative) are shown to the left (along with the average of energy difference from Vina, and those with worse Energy (less negative) are shown to the right along with their average energy difference.

![Binding energy first predicted mode](https://github.com/QVina/QVina.github.io/raw/master/qvina2 fig 4 binding energy.png)



It is also witnessed that QVina 2 is more accurate than GOLD 5.2 and is only slightly less accurate than Dock 6.6. This shows that QVina 2 has paved the way for some high-throughput and sufficiently accurate virtual screening of molecular libraries. This in turn brings great value to the fragment-based computer-aided drug design.

A good example of the quality of prediction of QVina 2 is 3PWW, shown in the below figure. 3PWW has 20 active bonds and 49 heavy atoms. Although it was accelerated in a lower rate than QVina 1 (4.74 versus 15.36 times), QVina 2 succeeded with RMSD of 1.436, while Vina, GOLD, Dock, and QVina 1 (not shown) all failed with respective RMSD values of 2.032, 2.711, 5.352, and 6.067). It is easy to notice the closeness between QVina 2 prediction in Red and the experimental data in Cyan as shown in the below figure.

![Example](https://github.com/QVina/QVina.github.io/raw/master/fig7 without caption.png)
Experimental (Cyan sticks), and QVina 2 (Red Sticks) are close to each other (except for the terminal double ring), while GOLD (Magenta lines) and Vina (Blue lines) conformations have flipped upper right and lower right branches and relatively distant left branch, and Dock (Yellow lines) has a totally flipped conformation. Part of the receptor was removed to show the ligands.


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


