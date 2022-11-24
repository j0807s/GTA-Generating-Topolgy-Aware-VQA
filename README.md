# GTA: Generating Topolgies-Aware Variational Quantum Algorithm for Quantum Ensemble
**GTA: Generating Topolgies-Aware Variational Quantum Algorithm for Quantum Ensemble**\
**_Junsu Kim_**, Suhyun Kim

## Abstract
Training Variational Quantum Algorithm (VQA) using real quantum machines is extremely slow due to waiting queue for cloud access at every training iteration and also suffers from noisy devices. To alleviate this, recent studies propose ensemble training with multiple quantum devices. Unfortunately, a transpiled circuit architecture (i.e., transpiled VQA) still varies depending on a topolgy of each quantum computer, exacerbating the performance of a given VQA on certain devices and may slowing down the convergence. Thus, we propose GTA that generates topologies-aware VQA for efficient training and constant performance on heterogenous quantum architectures.

## Installation

### Prerequisites
* python == 3.8
* ray == 2.1
* qiskit == 0.24.1

### Setup
* TBD

## Reproudce
Below commands save the best and the worst VQA circuit architecture based on given quantum devices (default: Lima, Oslo, Manila). Then, start training using multiple devices with the VQA. Finally, save loss function graphs and analyze performance on each device used in training.

```bash
sh run_vqe.sh
sh run_qml.sh
sh run_qaoa.sh
```

## Results
* Performance on each device: TBD 
* Ensembled loss: TBD



