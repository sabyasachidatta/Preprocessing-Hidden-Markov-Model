# Preprocessing-Hidden-Markov-Model

Task 1: # Preprocessing

Given the text file (grail.txt) from the Web Text Corpus of NLTK, perform the following tasks:
1. Report the number of sentences and tokens contained in the file given as input.
2. Convert the whole text to lower case and report the number of unique tokens present
before and after lower casing in the input file.
3. Report the number of stopwords in the file. Report the number of tokens left after
stopword removal.
4. Perform stemming after removing stopwords and report the number of unique tokens left
in the text.
5. Report the number of words starting with a consonant and the number of words starting
with a vowel in the file given after performing steps 1,2,3, and 4.
6. Given a word and a file as input, return the number of sentences starting with that word
in the input file after performing steps 1,2,3, and 4.

7. Given a word and a file as input, return the number of sentences ending with that word in
the input file after performing steps 1,2,3, and 4.
8. Given a word and a file as input, return the count of that word in the input file after
performing steps 1,2,3, and 4.

Task 2: # Hidden Markov Model

Implement an HMM-based approach to POS tagging. Specifically, you have to implement the
Viterbi algorithm using a bigram tag/state model. For training, a POS-tagged section of the
BERP corpus has been attached (Training set_HMM.txt). Your systems will be evaluated
against an unseen test set drawn from the same corpus.
Training: The training data consists of around 15,000 POS-tagged sentences from the BERP
corpus. The sentences are arranged as one word-tag pair per line with a blank line between
sentences, words and tags are tab-separated. Contractions are split out into separate tokens
with separate tags. An example is shown here:
I PRP
'd MD
like VB
french JJ
food NN
Assume that the tags and words that appear in the training data constitute all the tags that exist
(no new tags or words will appear in testing).
Decoding: For decoding, your system will read in sentences from a file with the same format
minus the Tags, ie, one word per line ending with a period and a blank line before the next
sentence. As output, you should emit an appropriate tag for each word in the same format as
the training data.
