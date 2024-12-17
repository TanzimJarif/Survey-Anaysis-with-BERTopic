This project performs topic modeling and text analysis on "The Kindness Test" dataset. It utilizes various techniques, including Latent Dirichlet Allocation (LDA), BERTopic, and statistical methods, to extract meaningful topics and insights.

Features
Preprocessing: Tokenization, POS tagging, and feature extraction using libraries such as NLTK and Gensim.
Topic Modeling:
LDA with Scikit-learn for traditional topic extraction.
BERTopic for advanced topic modeling using contextual embeddings.
Evaluation: Coherence scores to assess topic quality.
Visualization: Results are visualized with UMAP and other plotting techniques.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/topic-modelling-kindness-test.git
cd topic-modelling-kindness-test
Install required libraries:

bash
Copy code
pip install -r requirements.txt
Dataset
The project uses "The Kindness Test Clean Data v6.csv". Ensure the dataset is stored in the Dataset directory before running the notebook.

Getting Started
Load the dataset:

python
Copy code
filename = "Dataset/The Kindness Test Clean Data v6.csv"
kindness_data = pd.read_csv(filename, low_memory=False)
Select relevant columns for analysis, such as:

python
Copy code
receive_columns = ['receive_what', 'receive_type', 'receive_feel1', 'receive_feel2', 'receive_feel3']
receive_df = kindness_data[receive_columns]
Apply topic modeling techniques (e.g., LDA, BERTopic) and evaluate results.

Libraries Used
Basic Libraries: numpy, pandas, matplotlib, tqdm
Natural Language Processing: nltk, gensim
Machine Learning: scikit-learn
Topic Modeling: BERTopic, umap, hdbscan, sentence-transformers
Others: scipy, collections
