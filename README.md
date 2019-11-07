# Requirements
- python3.6
- tensorflow-gpu 1.11
   - GPU: `pip install tensorflow-gpu==1.11.0`
- tensorflow_hub 0.1.1
- nltk,numpy, pandas, json, sklearn


# Data / Models
The original dataset are from [dataset link](http://cseweb.ucsd.edu/~jmcauley/datasets.html), including Amazon QA and reviews data.
In our work, we have chosen 7 categories, namely Tools_and_Home_Improvement, Patio_Lawn_and_Garden, Automotive, Cell_Phones_and_Accessories, Health_and_Personal_Care, Sports_and_Outdoors, Home_and_Kitchen.
In order to replicate our results, you need to download QA and review dataset in all of these categories,but please feel free to run our model on different categories.
Pleae keep downloaded file in folder "data".

# Dataset preprocessing
python data_reprocess.py  

# Training
1. Cross-domain training FLTR
   python FLTR_1st.py
2. Fine-tuning FLTR for each category
   python FLTR_2rd.py
3. Cross-domian training BERTQA
   python BertQA.py 8
4. Fine-tunning BERTQA for each category
   python BertQA.py
   
# Prediction
  
# Publication

Zhang, Shiwei; Lau, Jay Han; Zhang, Xiuzhen; Chan, Jeffrey; Paris, Cecile. Discovering Relevant Reviews for Answering Product-related Queries. In: IEEE 19th International Conference on Data Mining; November 2019;  Beijing, China. ICDM; 2019.
