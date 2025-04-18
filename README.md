# Self-Supervised Style Transfer for Image Representation Learning

This project investigates the use of **style transfer** as a **self-supervised learning** technique to improve image representations for downstream tasks like classification. By combining contrastive learning with artistic stylization, this work introduces a novel way to learn semantically rich image embeddings without labels.

## 🎯 Objective

To enhance self-supervised representation learning using **artistic style transfer** and **contrastive learning** on a Siamese Network.  
We test whether applying different styles to the same content image improves a model’s ability to learn discriminative visual features.

## 🗃️ Datasets

- **COCO 2017** (for content images) – [COCO Dataset](https://cocodataset.org/)
- **WikiArt (Impressionism subset)** (for style images) – [WikiArt](https://www.wikiart.org/)

## 📊 Results

- **Siamese Network Accuracy:** ~77% on binary pair classification  
- **Linear Classifier Accuracy:** ~74%  
- High performance on negative class, lower on positive class due to class imbalance.

### 📉 Metrics Breakdown
- Accuracy: 73.68%  
- Precision (minority class): 20.00%  
- Recall (minority class): 5.88%

## 🔬 Literature Comparison

| Paper | Method | Accuracy |
|-------|--------|----------|
| Noroozi et al. (Jigsaw Puzzles) | Self-supervised CNN | 57.1% |
| Our Model | Style Transfer + Contrastive | **73.68%** |

### How to Run

1. Clone this repository.
2. Open the [`project.ipynb`](./project.ipynb) notebook in Jupyter or Colab.
3. Run all cells to perform training, evaluation, and visualization.

Or use our shared notebook directly:  
📎 [Colab Link](https://colab.research.google.com/drive/1squG15RDxChEe_0TzkH5P1tiFz6dWPq0?usp=sharing)

## 📝 Conclusion

This study successfully demonstrates that style transfer enhances contrastive learning in a self-supervised setting. While effective overall, improvements in class balancing and evaluation metrics could further refine results. Future work can involve deeper backbones, better sampling strategies, and evaluation on broader downstream tasks.

---

