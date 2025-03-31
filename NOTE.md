# NOTE

## RNA Knowledge:

### What is RNA?
RNA (Ribonucleic Acid) is a nucleic acid, a type of biological macromolecule, similar to DNA but with key differences in structure and function. It plays a crucial role in genetics and cellular biology.


## Articles:
- [US-align: universal structure alignments of proteins, nucleic acids, and macromolecular complexes](https://www.nature.com/articles/s41592-022-01585-1)
- [RNA-Puzzles Round V: blind predictions of 23 RNA structures](https://www.nature.com/articles/s41592-024-02543-9)
- [Ribonanza: deep learning of RNA structure through dual crowdsourcing](https://www.biorxiv.org/content/10.1101/2024.02.24.581671v2)
- [Thoughts on how to think (and talk) about RNA structure](https://www.pnas.org/doi/10.1073/pnas.2112677119)
- [Big data and deep learning for RNA biology](https://www.nature.com/articles/s12276-024-01243-w)
- [Machine learning modeling of RNA structures: methods, challenges and future perspectives](https://academic.oup.com/bib/article/24/4/bbad210/7190934)
- [Machine learning a model for RNA structure prediction](https://pmc.ncbi.nlm.nih.gov/articles/PMC7671377/)
- [Large language modeling and deep learning shed light on RNA structure prediction](https://www.nature.com/articles/s41592-024-02488-z)

- [RNA language models predict mutations that improve RNA function](https://www.nature.com/articles/s41467-024-54812-y)
- [RiboNucleic Acid Language Model - RiNALMo](https://github.com/lbcb-sci/RiNALMo)
- [RiNALMo: General-Purpose RNA Language Models Can Generalize Well on Structure Prediction Tasks](https://arxiv.org/abs/2403.00043)
- [Multi-purpose RNA language modelling with motif-aware pretraining and type-guided fine-tuning](https://www.nature.com/articles/s42256-024-00836-4)

## Extra
This is for research purpose

- [How to write a Research Paper](https://www.reddit.com/r/studytips/comments/1c71t74/effective_steps_for_writing_a_research_paper/)
- [How to Write a Research Paper](https://cambridge-research.org/blogs/how-to-write-a-research-paper/)
- 

```
1. Problem Definition & Scope
Objective: Predict the 3D structure of RNA from its sequence.

Scope:

Input: RNA sequence (nucleotides: A, U, G, C).

Output: 3D coordinates of RNA structure.

Challenges: Data scarcity, high-dimensionality, complex energy landscapes.

2. Literature Review & Benchmarking
Study existing RNA folding algorithms (e.g., RNAfold, Rosetta, EternaFold, AlphaFold-RNA).

Explore ML & Deep Learning models in protein folding (e.g., AlphaFold2).

Read papers on graph neural networks (GNNs), transformers, diffusion models in structural biology.

3. Data Collection & Preprocessing
3.1. Data Sources
Protein Data Bank (PDB) (https://www.rcsb.org): Download RNA structures.

RNACentral (https://rnacentral.org): Large database of non-coding RNA sequences.

Modomics (http://modomics.genesilico.pl): RNA modifications.

3.2. Feature Engineering
Primary Sequence Features: One-hot encoding, k-mer embedding.

Secondary Structure: Predicted with RNAfold, MFE, base-pairing probabilities.

3D Structural Features: Atomic coordinates, dihedral angles, torsion angles.

Graph Representation: Nodes (nucleotides), edges (base pairs, backbone).

4. Model Selection & Architecture
4.1. Classical ML Approaches
Random Forests, SVMs, XGBoost (for simpler folding pattern predictions).

Energy-based Models (Boltzmann distributions).

4.2. Deep Learning Approaches
Graph Neural Networks (GNNs): Treat RNA as a molecular graph.

Transformers (Attention models): Encode RNA sequence interactions.

Diffusion Models: Learn probabilistic folding pathways.

3D CNNs/Vision Models: If voxelizing 3D RNA structures.

4.3. Potential Architectures
GNN + Transformer Hybrid: For sequence & structure encoding.

AlphaFold-like Model: Predict 3D structure from pairwise distances.

5. Training & Optimization
Loss Functions:

Root Mean Square Deviation (RMSD) for 3D coordinates.

Graph similarity losses for structure comparison.

Free energy minimization constraints.

Training Strategy:

Supervised Learning: Train on labeled 3D RNA structures.

Self-Supervised Learning: Use contrastive learning on RNA pairs.

Reinforcement Learning: Optimize folding pathways.

6. Model Evaluation
Metrics:

Global Distance Test (GDT): For 3D accuracy.

TM-score: Structural similarity measure.

Energy-based Evaluation: Check stability.

Computational Efficiency: Time to predict folding.

Benchmark Against:

Experimental 3D structures.

Traditional RNA folding tools.

7. Deployment & Applications
Deploy the model via Python API (FastAPI, Flask).

Package into a web app for visualization (PyMOL, ChimeraX, 3Dmol.js).

Integrate into RNA drug discovery pipelines.

8. Further Research & Improvements
Integrate RNA modification effects.

Train on larger metagenomic datasets.

Use Quantum ML (QML) for energy minimization.

Next Steps
Start with a literature review on existing RNA folding ML models.

Collect RNA 3D structure data from PDB, RNAcentral.

Choose between Graph Neural Networks (GNNs) or Transformers.

Develop a baseline model (e.g., predicting secondary structure first).

Iterate on 3D folding prediction using GNNs, transformers, or diffusion models.
```
