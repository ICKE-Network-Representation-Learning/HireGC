###
This repository provides a reference implementation of *HireGC* as described in the [paper](HireGC: Hierarchical Inductive Network Representation Learning via Graph Coarsening.). 

#### **Required Packages**
* python 3.7
* tensorflow 1.15.0
* numpy 1.19.5
* scipy 1.7.3
* scikit-learn 0.20.3
* networkx 2.4
* theano 1.0.5
* torch 1.4.0

#### **How To Run Node Classification**
Use `python main.py` to run the code with all the default settings. Here are some useful arguments that can be passed to the program:
* `--data`: name of the dataset (file located in `./dataset`), e.g., `--data /cora`.
* `--basic-embed`: name of the base embedding method, e.g., `--basic-embed netmf`.
* `--coarsen-level`: number of levels for coarsening, e.g., `--coarsen-level 3`.
* `--embed-dim`: dimensionality for embedding, e.g., `--embed-dim 128`.
* `--refine-type`: refinement method, including `MD-gcn` , `MD-dumb` (without model training), and `MD-gs` (using GraphSAGE).

#### **How To Run Link Prediction**
Use `python linktrain.py` to run the code with all the default settings. Here are some useful arguments that can be passed to the program:
* `--data`: name of the dataset (file located in `./dataset`), e.g., `--data /cora`.
* `--basic-embed`: name of the base embedding method, e.g., `--basic-embed netmf`.
* `--coarsen-level`: number of levels for coarsening, e.g., `--coarsen-level 3`.
* `--embed-dim`: dimensionality for embedding, e.g., `--embed-dim 128`.
* `--learning-rate`: dimensionality for embedding, e.g., `--learning-rate 0.001`.
* `--refine-type`: refinement method, including `MD-gcn` , `MD-dumb` (without model training), and `MD-gs` (using GraphSAGE).


## **If you find *HireGC* useful in your research, please cite our paper:**
Zhao S, Xu C, Du Z, et al. HireGC: Hierarchical inductive network representation learning via graph coarsening[J]. Knowledge-Based Systems, 2025: 113058.
 
