# 🔤 NLP Text Preprocessing

The first step of any NLP pipeline: turning raw text into clean units a model can work with. This repo covers the classic preprocessing techniques with **NLTK**. They're the foundations behind the text chunking I later used in my RAG projects.

## 📓 Notebooks
| Notebook | What it covers |
|---|---|
| `Tokenization.ipynb` | Splitting a paragraph into sentences (`sent_tokenize`) and words (`word_tokenize`) |
| `Stemming VS Lemmetization.ipynb` | Reducing words to a root form with three stemmers (**Porter**, **Snowball**, **Regexp**) and comparing them with **WordNet lemmatization** |

## 💡 Key takeaway
- **Stemming** chops word endings by rule. It's fast but can produce non-words ("history" → "histori").
- **Lemmatization** uses a dictionary to return a real base word. It's slower but more accurate, and better when the meaning matters, as in chatbots and search.

## 🚀 Run it
```bash
pip install nltk jupyter
python -c "import nltk; nltk.download('punkt'); nltk.download('wordnet')"
jupyter notebook
```

## 🔮 Next
Stop-word removal, Bag-of-Words, TF-IDF and word embeddings.

---
👩‍💻 **Nidhi Mehta** · [GitHub](https://github.com/itsnidhimehta)
