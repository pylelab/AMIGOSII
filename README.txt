AMIGOS II v1.0.1
*** AMIGOS II Installation ***

AMIGOS II uses java, which can be installed from 
https://www.java.com/en/download/manual.jsp
Please do NOT unzip the amigos2.jar file in this folder.

*** AMIGOS II Usage ***

Launch AMIGOS II using the "amigos2.bat" script on Windows or the 
"amigos2.sh" script on other Operating Systems.

First, load PDB files with File-->open PDB... One or more files in a
directory can be loaded.

You will now have one or more expandable "trees" that display the RNA
residues in the loaded structures.

** Plotting

Eta-theta plots can be generated with Plot-->draw plot. "All
nucleotides" plots all defined eta-theta coordinates for the loaded
nucleotides, and "Selected" plots those selected in the tree
hierarchy.

Nucleotides with specific sugar puckers can be shown with
Plot-->options-->show only.

Nucleotides on the plot can be selected by mouse-clicking if in "point
select" mode (bottom right drop-down).

The plot can be zoomed/unzoomed if in "zoom box" mode. Click and drag
a box on the plot and then click the + magnifying glass button in the
lower right.


** Getting coordinates and torsions for a nucleotide

Select a nucleotide in the tree hierarchy and click the bottom-left
button (the info bubble). This will output (in the upper-left box) the
eta-theta coordinates, the sugar pucker phase and nominal sugar
pucker, and the standard torsion angles for the nucleotide.


** Performing a worm search

A PRIMOS search can be performed within AMIGOS II.

Select a continuous stretch of nucleotides in the tree hierarchy
(either shift-click or ctrl-click with the mouse).

Click the 2nd button on the lower left (binoculars). This will
generate PRIMOS-like output, sorted with the best matches at the top.

This table can easily be copied and pasted to a spreadsheet or file if
desired.

** Finding known motifs (e.g. GNRA-like) without a probe

It is first necessary to load one or more motif templates into AMIGOS
II. Examples reside in the motifs subfolder.

So, do File-->load motif templates... and select one or more of the
files from this directory.

The structure of the template looks like this:

# canonical strand of kink-turn motif
Kink-turn
155.0 25.0 165.0 25.0
200.0 30.0 75.0 20.0
10.0 30.0 340.0 30.0
165.0 30.0 130.0 30.0
193.0 20.0 230.0 30.0

Lines at the top starting with # are read as comments. The next line
is a name/label for the motif. 

The lines that follow designate permissible eta-theta values and
ranges for the motif in question. Here, the kink-turn is defined with
4 eta-theta coordinates. For example, the (155.0 25.0 165.0 25.0) line
states that the first nucleotide has eta = 155 +/- 25 and theta = 165
+/- 25.

You can define your own motif templates by following these examples.

Once PDB files and motif templates are loaded into AMIGOS II, click
the 3rd button on the lower left (the binoculars with the globe). You
can now choose what you want to find, and AMIGOS II will output
stretches of nucleotides that match the template from the loaded PDB
files


** Viewing the structure of a stretch of nucleotides

AMIGOS II has a rudimentary structure viewer built-in. Select a
stretch of nucleotides of interest in the hierarchy (shift-click or
ctrl-click) -- this could be, for example, the output from a PRIMOS
search.

Click the 4th button on the lower left (magnifying glass). This will
show the 3-D structure of the selected nucleotides. 

** Sequence search

Clicking the 5th button on the lower left ("AC") will prompt for a
sequence. Entering a sequence and clicking OK will show all
occurrences of that continguous sequence in the loaded structures.
