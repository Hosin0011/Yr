# import nltk
from nltk.tokenize import word_tokenize
from nltk.probability import FreqDist

nltk.download('punkt')
text = "This is a sample text for NLP analysis."

tokens = word_tokenize(text.lower())
fdist = FreqDist(tokens)

print("Tokenized Text:", tokens)
print("Word Frequencies:", fdist.most_common())
