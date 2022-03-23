all : lexicon.lexd \
	gen.hfst

lexicon.lexd : morphology.lexd
	cat morphology.lexd > lexicon.lexd

gen.att : lexicon.lexd
	lexd <lexicon.lexd >gen.att

gen.hfst : gen.att
	hfst-txt2fst <gen.att >gen.hfst
