# Storage Capacity in Biologically Plausible Hopfield Networks

## Overview

This repository contains the code and resources for the project titled **"Storage Capacity in Biologically Plausible Hopfield Networks"**. This project, conducted by Maria Yuffa Meshcheryakova and Elizaveta Shegurova, is part of the coursework for the NX-465 course on Computational Neurosciece: Neuronal Dynamics. The primary focus of the project is to explore the storage capacity and retrieval accuracy of different configurations of Hopfield networks under biologically realistic constraints.

## Project Structure

- **`Code_MP1_MariaYuffa_ElizavetaShegurova/`**: Contains the Jupyter notebooks used for implementing and experimenting with different Hopfield network models.
  - **`Ex0+1.ipynb`**: Initial experiments focusing on the standard Hopfield model.
  - **`Ex2.ipynb`**: Experiments involving biologically realistic features, including sparsity and asymmetric connectivity.
  - **`ex3_final.ipynb`**: Final set of experiments integrating all features and analyzing network performance.
- **`Report_MP1_MariaYuffa_ElizavetaShegurova.pdf`**: The detailed report outlining the methodology, results, and conclusions of the project.
- **`.DS_Store`**: A system file that can be ignored or removed.

## Introduction

In this project, we extend the classical Hopfield network model to incorporate biologically plausible features such as:

1. **Sparse Neuronal Activity**: Reflecting the realistic scenario where only a small percentage of neurons are active at any given time.
2. **Asymmetric Connectivity**: Implementing Dale’s law by ensuring that each neuron’s synapses are either exclusively excitatory or inhibitory.
3. **Separate Excitatory and Inhibitory Populations**: Dividing neurons into groups with distinct roles to better simulate biological neural networks.

These modifications aim to investigate how these biological constraints affect the memory storage capacity and pattern retrieval accuracy of the network.

## Methods and Models

### Standard Hopfield Network
- **Symmetric Connectivity**: Neurons are connected with symmetric weights, and patterns are stored with equal activity across the network.
- **Balanced Random Patterns**: A traditional approach with 50% of neurons active.

### Modified Networks
- **Low-Activity Patterns**: Simulating sparse neuronal firing, more reflective of actual brain activity.
- **Excitatory/Inhibitory Neuron Populations**: Incorporating Dale's law by ensuring that each neuron is either excitatory or inhibitory but not both.

### Experiments and Evaluation
- **Memory Storage Capacity**: The maximum number of patterns that can be accurately retrieved from the network.
- **Pattern Retrieval Accuracy**: Evaluated using metrics such as Hamming distance and pattern overlap.

## Results

- The **standard Hopfield network** could store a significant number of patterns but struggled with retrieval accuracy as the number of stored patterns increased.
- The introduction of **sparse activity** improved storage capacity, as fewer overlapping patterns reduced interference.
- Incorporating **excitatory and inhibitory populations** enhanced the network's overall capacity but made it more challenging to maintain accurate pattern retrieval due to increased complexity.

## Conclusion

Our findings suggest that introducing biologically realistic features into Hopfield networks can significantly impact their performance. Sparse activity and distinct excitatory/inhibitory populations improve storage capacity but require careful balancing to maintain retrieval accuracy. This project underscores the importance of considering biological constraints when modeling neural networks to better understand the balance between storage capacity and retrieval accuracy.

## How to Run the Code

1. Clone the repository:
   ```bash
   git clone https://github.com/username/project-repo.git
   ```
2. Navigate to the `Code_MP1_MariaYuffa_ElizavetaShegurova/` directory.
3. Open the Jupyter notebooks (`.ipynb` files) using Jupyter Notebook or Jupyter Lab.
   ```bash
   jupyter notebook
   ```
4. Run the notebooks to reproduce the experiments and results.

## Dependencies

Ensure you have the following Python packages installed:
- `numpy`
- `matplotlib`
- `scipy`
- `jupyter`

You can install the required packages using:
```bash
pip install numpy matplotlib scipy jupyter
```

## Authors

- **Maria Yuffa Meshcheryakova**
- **Elizaveta Shegurova**

For more detailed information, please refer to the full project report available in the `Report_MP1_MariaYuffa_ElizavetaShegurova.pdf` file.
