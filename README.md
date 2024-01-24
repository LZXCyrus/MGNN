# MGNN

MGNN is a deep learning framework to use multimodal stock related data for tracking stock movements. The framework has been proven to outperform traditional methods in predicting stock prices, making it a valuable tool for providing valuable insights for investors.

## 📝 Updates


## 📊 Preparing Datasets

Our multimodal dataset includes financial news,fundamental and stock relationship data. We provide 200 training data samples of financial news and fundamental data in this repo. 

#### 1. financial news and fundamental data
The structure of a dataset is a dict consisting of four field: `stock_code`, `date` and `news` and `fundamental`.The field `fundamental` is a dict with `high`, `open`, `low`, `close` and `num`.

Here is an example.
```
{
  "stock_code": "601939",
  "date": "2018-05-02",
  "news": "近日，中国建设银行与华南城集团在广西南宁签订住房租赁业务战略合作框架协议。据双方战略合作协议，建设银行和华南城集团将在住房租赁和普惠金融等方面展开深度合作。"
  "fundamental": {
                  'high': 7.61 ,
                  'low': 7.39 ,
                  'open': 7.58 ,
                  'close': 7.47,
                  'num': 95696669
                 },
}
```


#### 2. stock relation data
The industry stock relation data is an adjacent matrix $\mathbb{R}^{N×N}$, where $N$ represents the number of stocks. It can be collected from the Chinese Stock Market & Accounting Research (CSMAR) database.


## ⚙️ Requirements

We will provide the detailed requirements in `requirements.txt`. You can run pip install requirements.txt to create the same running environment as ours:

```bash
conda create -n MGNN python=3.8
conda activate MGNN
pip install -r requirements.txt
```
## 📚 Citation

