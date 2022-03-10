# Klingon Nouns

In this assignment, your task is to correctly implement Klingon nouns, as described in Chapter 3 of *The Klingon Dictionary* by Marc Okrand. In this assignment, you should **not** implement compound nouns (as described in Section 3.2.1), and you should **not** implement nouns created from verbs (as described in Section 3.2.2).

For each part, you are provided with a tsv file containing the expected pairs for that part. It is your responsibility to create a Makefile to test your output against the expected output.


## Part D (60%)

* In partD.lexc, your task is to implement Klingon nouns from Chapter 3, excluding words for body parts and language users. Implement Type 1 suffixes. From Type 2 suffixes, implement -mey only. Do not use -mey for words that are inherently plural. You may use flag diacritics.


## Part C (13%)

* In partC.lexc, your task is implement Klingon nouns from Chapter 3, including words for body parts and language users. Implement Type 1 and Type 2 suffixes. Do not allow any plural suffixes for inherently plural nouns. You should allow the use of -mey with the singular variant of inherently plural nouns, nouns representing body parts, and nouns representing language users, but such cases must also be marked as +Scattered. You must use flag diacritics.


## Part B (13%)

* In partB.lexc, your task is to extend your implementation of Klingon nouns to implement all Type 1, Type 2, Type 3, Type 4, and Type 5 suffixes. Do not allow the use of the locative suffix for the Klingon words for "hereabouts" or "everywhere". You must use flag diacritics.



## Part A (14%)

* In partA.foma, define a named network called IPA. The upper side of this network should allow strings made up of letters from the Klingon alphabet. The network should map Klingon letters to their IPA equivalents. Any symbols not in the Klingon alphabet should map to themselves. Tokenization must be implemented such that the sequence 'ngh' maps to 'nɣ' not 'ŋh'. See alphabet.tsv.

* In partA.foma, load your partB.lexc file and save it as a network called Lexicon.

* In partA.foma, define a network called LexiconLowerIPA. If you run pairs on LexiconLowerIPA, the lower side of the lexicon should be in IPA.

* In partA.foma, define a network called LexiconUpperIPA. If you run pairs on LexiconUpperIPA, the noun roots on the upper side of the lexicon should be in IPA.

* In partA.foma, define a network called LexiconIPA. If you run pairs on LexiconIPA, the noun roots on the upper side of the lexicon should be in IPA, as should the entire word on the lower side.

