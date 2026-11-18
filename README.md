# AI / ML Portfolio

Coursework implementations and experiments from Computer Engineering studies at Sharif University of Technology, covering classical AI, reinforcement learning, machine learning, NLP, and deep generative models.

This repository is a portfolio of academic implementations and experiments. Individual notebooks may follow course-provided templates or collaborative coursework; see each notebook for its own attribution and requirements.

## Repository map

```text
AI-ML/
├── AI/
│   ├── CSP/                 # Sudoku, constraint satisfaction, graph coloring
│   ├── HC-Astar/            # A* search, hill climbing, simulated annealing
│   ├── Minimax/             # Connect Four game AI and Minimax
│   ├── RL/                  # Q-learning, SARSA, Monte Carlo, value iteration
│   └── Computer_Simulation/ # Smart-grid demand, queues, supply and outages
├── Ml/
│   ├── Classification/      # PCA, clustering, KNN and ensemble classifiers
│   ├── DGM/                 # WaveNet, graph VAE, CVAE, flows, inpainting, EBM
│   ├── NLP/                 # Skip-gram, Transformer, BERT and LoRA
│   ├── NeuralNetworks/      # MLP, backpropagation and optimizers
│   └── Regression/          # Perceptron, regression and regularization
├── requirements.txt
└── README.md
```

## Selected work

### Classical AI and search
- Constraint-satisfaction problems: Sudoku, backtracking, CP-SAT, AC-3/AC-4 and graph coloring.
- Informed and local search: A*, hill climbing and simulated annealing.
- Game AI: Connect Four with Minimax and alpha-beta pruning, including a board-rotation rule.

### Reinforcement learning
- Q-learning, SARSA and first-visit Monte Carlo on Gym environments such as FrozenLake and Taxi.
- Grid-world value-function and action-value calculations, Bellman-equation verification and optimal-policy extraction.

### Machine learning and optimization
- PCA and clustering (K-means, hierarchical clustering).
- KNN, Random Forest, Bagging and AdaBoost classification.
- MLP implementation, forward/backpropagation, SGD, momentum and Adam.

### NLP and language models
- Skip-gram / Word2Vec and FastText.
- Transformer components and model training.
- BERT full fine-tuning, parameter-efficient LoRA fine-tuning and few-shot classification experiments.

### Deep generative modelling
- WaveNet for autoregressive raw-audio modelling.
- Temporal Graph VAE for evolving graph sequences.
- Conditional VAE for image generation.
- RealNVP-like normalizing flows and image inpainting.
- Exploratory energy-based modelling and score-matching exercises.

### Smart-grid simulation
`AI/Computer_Simulation/Project.ipynb` implements a time-varying demand and supply simulation with consumer arrivals, queue admission, renewable/fossil supply, outage scenarios and comparisons of queue policies. It also explores Q-learning-based control; the notebook documents overfitting in that experiment, so it is presented as an exploration rather than a successful optimized controller.

## Setup

The root `requirements.txt` currently contains the basic scientific Python and notebook dependencies:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

On Windows PowerShell, activate with:

```powershell
.venv\Scripts\Activate.ps1
```

Some notebooks require additional project-specific packages not included in the root requirements file, including PyTorch, TensorFlow, torchvision, Gym/Gymnasium, Transformers, PEFT, librosa, gensim or fasttext. Install the dependencies required by the notebook you intend to run.

## Notes on reproducibility

- Some notebooks use external datasets or Google Drive paths; update those paths before running locally.
- Deep generative-model notebooks may require GPU resources and pretrained checkpoints.
- The repository contains coursework notebooks; results and implementation completeness vary by assignment. Consult each notebook's outputs, comments and TODO sections before treating an experiment as a final benchmark.

## Author

[Sorush Hatefi Vakilzadeh](https://github.com/Sorush-vh)
