# GTA: Generating Topolgies-Aware Variational Quantum Algorithm for Quantum Ensemble Training
**GTA: Generating Topolgies-Aware Variational Quantum Algorithm for Quantum Ensemble Training**\
**_Junsu Kim_**, Suhyun Kim

<p align="center">
<img src="Observation.png" width="100%">
</p>


<p align="center">
<img src="GTA1.png" width="100%">
</p>

## Abstract
Training Variational Quantum Algorithm (VQA) using real quantum machines is extremely slow due to waiting queue for cloud access at every training iteration and also suffers from noisy devices. To alleviate this, recent studies have proposed ensemble training with multiple quantum devices. Unfortunately, a transpiled circuit architecture (i.e., transpiled VQA) still varies depending on a topolgy of each quantum computer, exacerbating the performance of a given VQA on certain devices and may slowing down the convergence. Also, if a noise level of a device when inferencing is different from the noise level during training, the learned parameters can not guide to optimal solution. Thus, we propose GTA, which generates topologies-aware VQA for efficient training and constant performance on heterogenous quantum architectures. GTA first observes what device is more accessible and provides better fidelity by caputuring the queue position of each device and the noise configuration. After selection of the primary architecture, GTA optimizes the given VQA to the primary architecture, reducing SWAP gates. During ensemble training, if noise levels vary depending on transpiled circuits and quantum machines, GTA introduces more noise by gate insertion (e.g., two Pauli X gates) to adjust their noise levels to the primary one. When inferencing using a single quantum device, GTA also introduces noise to obtain optimal solution.

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



