## Optimizing Image Classification on CIFAR-10 with Transformer Architectures

### Overview
This repository contains the final report and supporting materials for my Data Mining course project at Columbia University. My team explored the application of Transformer architectures to image classification tasks, using the CIFAR-10 dataset as a benchmark. The primary focus was on balancing computational efficiency with classification accuracy by comparing various Transformer-based models.

### Key Highlights
- **Architectures Evaluated**: Vision Transformer (ViT), Performer variants (ReLU, ELU, GELU, Exponential), and a novel Performer-fθ with learnable kernel functions.
- **Dataset**: CIFAR-10, with 60,000 images across 10 classes.
- **Metrics**: Training time, inference time, classification accuracy, and computational efficiency.

### Contributions
- **Comparative Analysis**: Explored trade-offs between computational efficiency and classification accuracy across different architectures.
- **Innovative Approaches**:
  - Performer-fθ: A novel variant using a learnable kernel function to improve attention mechanism flexibility and performance.
  - Efficient Kernel Implementations: Experimented with ReLU, exponential, and other approximations to address the quadratic complexity of traditional attention mechanisms.
- **Performance Results**:
  - Performer-GELU achieved the highest accuracy (88.64%).
  - Performer-ReLU provided the best balance of speed and accuracy (87.39% accuracy with linear complexity).
  - Performer-EXP demonstrated robust efficiency, achieving 86.17% accuracy with significantly (>2x) faster training times.

### Structure
The repository includes:
1. **Report**: A detailed breakdown of our methodologies, experiments, and results.
2. **Code**: Implementation of each Transformer variant, along with hyperparameter optimization pipelines using Grid Search and Optuna.
3. **Figures and Results**: Visualizations of training dynamics, loss curves, and model comparisons.

### Future Directions
- Expand testing to larger datasets (e.g., CIFAR-100, ImageNet) to evaluate scalability.
- Further refine learnable kernel functions like fθ for improved accuracy and efficiency.
- Explore automated hyperparameter tuning frameworks for broader generalization.
