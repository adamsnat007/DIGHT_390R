all : lexicon.lexc \
	gen.hfst

lexicon.lexc : root.lexc morphology.lexc adjectives.lexc nouns.lexc pronouns.lexc prepositions.lexc punctuation.lexc articles.lexc
	cat root.lexc morphology.lexc > lexicon.lexc #adjectives.lexc nouns.lexc pronouns.lexc prepositions.lexc punctuation.lexc articles.lexc > lexicon.lexc

gen.hfst : lexicon.lexc
	hfst-lexc <lexicon.lexc >gen.hfst
