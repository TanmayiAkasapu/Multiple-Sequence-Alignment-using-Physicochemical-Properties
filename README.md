# Multiple-Sequence-Alignment-using-Physicochemical-Properties
A multiple sequence alignment using a star alignment strategy to align remote homologous protein sequences via physicochemical properties.

Physicochemical alignments are similar to standard alignments with a few main differences. They are physicochemical equivalency alignments. In other words, they will only directly correspond to the true evolutionary path when the physicochemical properties selected for at each residue position are known. However, some of the more fundamental physicochemical properties have proven to be good general indicators; most notably molecular weight and hydrophobicity.

==========================================================================================================================================

Visuals:
<img width="1490" height="59" alt="image" src="https://github.com/user-attachments/assets/5fee29d0-b6f2-4b3b-ac17-2739b4ebf8fa" />

==========================================================================================================================================

Installation Instructions:
To install PCDTW (Two Options): -Use ‘pip install PCDTW’ in a powershell prompt -Use ‘!pip install PCDTW’ in a jupyter notebook
To use PCDTW: Use ‘import PCDTW’

==========================================================================================================================================

Usage:
FASTALoc=Fasta file location as a string

MSAAlignment=PCDTW.PCDTWMSAlign(FASTALoc, PCProp1='Mass', PCProp2='HydroPho', n_jobs=-1)
print(MSAAlignment[0]) --> Gives the output as a list of aligned sequences
print(MSAAlignment[1]) --> Gives the output in Fasta format

PCProp1/PCProp2 options:
'HydroPho'
'HydroPhIl'
'Hbond'
'SideVol'
'Polarity'
'Polarizability'
'SASA'
'NCI'
'Mass'
'None'

n_jobs options:
-1 use all available cores
Integer 1 or greater specifies the number of cores to use
