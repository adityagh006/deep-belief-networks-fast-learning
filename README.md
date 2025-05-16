# Fast Learning for Deep Belief Networks

Implementation of the seminal paper ["A Fast Learning Algorithm for Deep Belief Nets"](https://www.cs.toronto.edu/~hinton/absps/fastnc.pdf) by Geoffrey Hinton, Simon Osindero, and Yee-Whye Teh.

## 📖 Paper Summary
Deep Belief Networks (DBNs) are generative models composed of stacked Restricted Boltzmann Machines (RBMs). This project demonstrates:
- Greedy layer-wise pre-training
- Contrastive Divergence for RBM training
- Fine-tuning with backpropagation

Key contributions:
- Solving the vanishing gradient problem
- Effective weight initialization
- Efficient unsupervised learning

## 🛠️ Implementation Details
- **RBM Layer**: Binary and Gaussian units with Contrastive Divergence
- **DBN**: Greedy layer-wise stacking of RBMs
- **Optimization**: Adam optimizer with early stopping based on reconstruction error
- **Fine-tuning**: Supervised backpropagation (optional)

## 🖼️ Results
- Significant improvements with pre-training
- Visualizations of reconstructed images
- Comparison of performance with/without pre-training

## 📦 Usage
```bash
# Clone the repo
git clone https://github.com/adityagh006/deep-belief-networks-fast-learning.git
cd deep-belief-networks-fast-learning

# Install dependencies
pip install -r requirements.txt

# Run the training script
python train_dbn.py
