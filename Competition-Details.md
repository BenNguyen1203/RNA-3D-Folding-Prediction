## Rules
Submission are scored using [TM-score](https://www.kaggle.com/code/metric/ribonanza-tm-score), which goes from 0.0 to 1.0 (higher is better)

The rotation and translation of predicted structures to align with experimental reference structures are carried out by [US-align](https://www.nature.com/articles/s41592-022-01585-1). To match default settings, as used in the CASP competitions, the alignment will be sequence-independent.

For each target RNA sequence, you will submit 5 predictions and your final score will be the average of best-of-5 TM-scores of all targets. For a few targets, multiple slightly different structures have been captured experimentally; your predictions' scores will be based on the best TM-score compared to each of these reference structures.

Submission File
For each sequence in the test set, you can predict five structures. Your notebook should look for a file test_sequences.csv and output submission.csv. This file should contain x, y, z coordinates of the C1' atom in each residue across your predicted structures 1 to 5:
```
ID,resname,resid,x_1,y_1,z_1,... x_5,y_5,z_5
R1107_1,G,1,-7.561,9.392,9.361,... -7.301,9.023,8.932
R1107_2,G,1,-8.02,11.014,14.606,... -7.953,10.02,12.127
etc.
```
You must submit five sets of coordinates.

## Code Requirements
Submissions to this competition must be made through Notebooks. In order for the "Submit" button to be active after a commit, the following conditions must be met:

CPU Notebook <= 8 hours run-time
GPU Notebook <= 8 hours run-time
Internet access disabled
Freely & publicly available external data is allowed, including pre-trained models
Submission file must be named submission.csv
Submission runtimes have been slightly obfuscated. If you repeat the exact same submission you will see up to 5 minutes of variance in the time before you receive your score.

## Citation
Shujun He, CASP16 organizers, CASP16 RNA experimentalists, RNA-Puzzles consortium, VFOLD team, Rachael Kretsch, Alissa Hummer, Andrew Favor, Walter Reade, Maggie Demkin, Rhiju Das, et al. Stanford RNA 3D Folding. https://kaggle.com/competitions/stanford-rna-3d-folding, 2025. Kaggle.


Articles:
[US-align: universal structure alignments of proteins, nucleic acids, and macromolecular complexes](https://www.nature.com/articles/s41592-022-01585-1)
