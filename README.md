Code for the ACL 2021 paper "[Compare to The Knowledge: Graph Neural Fake News Detection with External Knowledge](https://aclanthology.org/2021.acl-long.62/)"


1. Pull the code and unzip the file inside fakeNews folder

2. Get the dataset from the link: https://github.com/BUPT-GAMMA/CompareNet_FakeNewsDetection/releases/tag/dataset

3. Make the data folder as the following
```
FakeNewsDetection
├── README.md
├── *.py
└───models
|   └── *.py 
└───data
    ├── fakeNews
    │   ├── adjs
    │   │   ├── train
    │   │   ├── dev
    │   │   └── test
    │   ├── fulltrain.csv
    │   ├── balancedtest.csv
    │   ├── test.xlsx
    │   ├── entityDescCorpus.pkl
    │   └── entity_feature_transE.pkl
    └── stopwords_en.txt

```



# Dependencies

Our code runs on the GeForce RTX 4080 (16GB), with the following packages installed:
```
python 3.8
torch 2.0.1 (with cuda 12.2)
nltk 3.4.5
tqdm
numpy
pandas
matplotlib
scikit_learn
xlrd (pip install xlrd)
seaborn
```



# Run

Train and test,
```
python main.py --mode 0
```

Test,
```
python main.py --mode 1 --model_file MODELNAME
```

