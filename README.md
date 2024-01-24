# MGNN

MGNN is a deep learning framework to use multimodal stock related data for tracking stock movements. The framework has been proven to outperform traditional methods in predicting stock prices, making it a valuable tool for providing valuable insights for investors.

## 📝 Updates


## 📊 Preparing Datasets

Our multimodal dataset includes financial news,fundamental and stock relationship data. We provide 200 training data samples of financial news and fundamental data in this repo. 

#### 1. data.jsonl
The structure of a dataset is a dict consisting of three field: `stock code`, `date` and `content`.The field `content` is a list of dict with image_id, fpath, im_height, im_width and category_id.

Here is an example.

#### 2. stock relation
The industry stock relation data is an adjacent matrix $\mathbb{R}^{N×N}$, where $N$ represents the number of stocks. It can be collected from the Chinese Stock Market & Accounting Research (CSMAR) database.


## ⚙️ Requirements

We will provide the detailed requirements in requirements.txt. You can run pip install requirements.txt to create the same running environment as ours:

```bash
conda create -n MGNN python=3.8
conda activate MGNN
pip install -r requirements.txt
```
## 📚 Citation

