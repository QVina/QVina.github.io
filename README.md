
<h1>Welcome to QuickVina!</h1>

QuickVina-W
--------------

We present QVina-W, a new docking tool particularly useful for wide search space, especially for blind docking. QVina-W utilizes the powerful scoring function of AutoDock Vina, the accelerated search of QVina 2, and adds thorough search for wide search space. It is based on the observation that allowing a searching thread to communicate with other nearby threads to make use of their wisdom, would increase the speed and sensitivity of that searching thread. This communication was allowed by means of a global buffer that keeps high quality search history points from all the threads.

In order to prove our theory, we analyzed the search process to trace the Average Sum of Proximity relative Frequencies (ASoF) among all searching threads, along with its effect on the speed and sensitivity of decision taking, as well as the effect on increasing number of search steps on the search speed and accuracy. That proved the direct relation between the length of the search and ASoF, which is reflected on the search speed and accuracy, and that in turn implies higher probability for better results. QVina-W makes use of the acceleration and explores four folds the number of points that Vina used to explore in a more efficient way. We also multithreaded the preparation overhead, which adds more to the overall time acceleration.

QVina-W proved to be faster than QVina 2 (with average and maximum normalized overall time accelerations of 3.60 and 34.33 folds in relation to Vina versus 1.98 and 18.02 respectively), yet better than Vina in terms of Binding Energy (78% of predictions with binding energy better than or equal to Vina) and RMSD (with success rate of 72% by QVina-W versus 63% by Vina).

![RMSD](https://github.com/QVina/QVina.github.io/raw/master/Figure 10.jpg)

RMSD of Vina, QVina 2, and QVina-W. Relative frequency of successes using RMSD to experimental data for both Vina and QVina-W. 
(A) RMSD distribution of the first mode. (B) First mode success at 2.0 A. (C) RMSD distribution of the best mode. (D) Best mode success at 2.0 A.



![Acceleration](https://github.com/QVina/QVina.github.io/raw/master/fig11.jpg)

Acceleration of QVina 2 and QVina-W (different steps) against Vina. (A) Overall time acceleration for QVina 2 and QVina-W steps X1, X2, X4 against Vina. (B) Normalized overall time acceleration for QVina 2 and QVina-W.




To cite QuickVina-W please cite:

__"Protein-Ligand Blind Docking Using QuickVina-W With Inter-Process Spatio-Temporal Integration"__
Nafisa M. Hassan, Amr A. Alhossary, Yuguang Mu & Chee-Keong Kwoh. Nature Scientific Reports 7(1) (2017). [DOI:10.1038/s41598-017-15571-7](http://dx.doi.org/10.1038/s41598-017-15571-7)


Quick Vina 2
-------------
Quick Vina 2 is a fast and accurate molecular docking tool, attained at accurately accelerating AutoDock Vina. It was tested against 195 protein–ligand complexes that compose the core set of the 2014 release of the PDBbind using default exhaustiveness level of 8, QVina 2 successfully attained up to 20.49-fold acceleration over Vina. The Pearson’s correlation coefficient between Vina’s QVina 2’s binding energy was 0.967 for the first predicted mode and 0.911 for the sum of all predicted modes.

The following figure shows the binding energies of the first predicted modes in QVina 1 and 2 on the vertical axis, against their corresponding modes in original Vina on the horizontal axis. The binding Energies of QVina 2 are almost identical to those of Vina. The Pearson’s correlation coefficient (r) for the two pairs was 0.967 between Vina and QVina 2, while it was only 0.780 between Vina and QVina 1. The same observation was also observed for the sums of all predicted modes where the respective values were 0.912 and 0.637

![Binding energy](https://github.com/QVina/QVina.github.io/raw/master/qvina2 fig 3 binding energy.png)

Next, the first predicted mode of binding energy is shown in the following figure.70% of first predicted binding energy modes from QVina 2 are equal to or better than Vina predicted modes. Even the remaining 30% have an average Energy difference as small as 0.58 Kcal/mol. On the contrary, the ratio is almost reversed for QVina 1: Only 37% are equal to or better than the Original Vina, and the remaining 63% have an average E difference as far as 1.56 Kcal/mol. Percentage of predictions with the same Binding Energies is shown in the middle part, while those with better Energy (more negative) are shown to the left (along with the average of energy difference from Vina, and those with worse Energy (less negative) are shown to the right along with their average energy difference.

![Binding energy first predicted mode](https://github.com/QVina/QVina.github.io/raw/master/qvina2 fig 4 binding energy.png)




It is also witnessed that QVina 2 is more accurate than GOLD 5.2 and is only slightly less accurate than Dock 6.6. This shows that QVina 2 has paved the way for some high-throughput and sufficiently accurate virtual screening of molecular libraries. This in turn brings great value to the fragment-based computer-aided drug design.

A good example of the quality of prediction of QVina 2 is 3PWW, shown in the below figure. 3PWW has 20 active bonds and 49 heavy atoms. Although it was accelerated in a lower rate than QVina 1 (4.74 versus 15.36 times), QVina 2 succeeded with RMSD of 1.436, while Vina, GOLD, Dock, and QVina 1 (not shown) all failed with respective RMSD values of 2.032, 2.711, 5.352, and 6.067). It is easy to notice the closeness between QVina 2 prediction in Red and the experimental data in Cyan as shown in the below figure.

![Example](https://github.com/QVina/QVina.github.io/raw/master/fig7 without caption.png)

Experimental (Cyan sticks), and QVina 2 (Red Sticks) are close to each other (except for the terminal double ring), while GOLD (Magenta lines) and Vina (Blue lines) conformations have flipped upper right and lower right branches and relatively distant left branch, and Dock (Yellow lines) has a totally flipped conformation. Part of the receptor was removed to show the ligands.


To cite QuickVina 2 please cite:

__"Fast, Accurate, and Reliable Molecular Docking with QuickVina 2"__
Amr Alhossary, Stephanus Daniel Handoko, Yuguang Mu, and Chee-Keong Kwoh. Bioinformatics (2015) 31 (13): 2214-2216. [DOI:10.1093/bioinformatics/btv082](https://doi.org/10.1093/bioinformatics/btv082)





## Important note:
* If you Don't know the Docking site, then QuickVina-W is your choice with the ability to dock a _WIDE_ search box.
* However if you _know_ the target search box, we recommend that you use QuickVina 2.


Having any inquiries, please contact us<br>
<a href= "mailto:aalhossary@pmail.ntu.edu.sg"> Amr Alhossary </a> <br>
<a href= "mailto:nafisa.mohamed@ntu.edu.sg"> Nafisa Mohamed </a> <br>


Your feedback is highly appreciated. We hope to hear from you soon!


