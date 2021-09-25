# Hebrew_lexicon
Biblical Hebrew Lexicon after Strong. Part of the resource “Biblical Hebrew for linguists: Westminster Leningrad Codex & Hebrew Lexicon” at https://lex.ibc.oarc.science. English part of a multilingual suite.

generate by:

`git clone https://github.com/ibc-oarc/Hebrew_lexicon_template ; ls ; rm -rf Hebrew_lexicon_template/.git ; rsync -a Hebrew_lexicon_template/ . --remove-source-files ; rm -rf Hebrew_lexicon_template/ ; pip install -r requirements.txt ; cd _data ; python precompile_lexicons.py ; python precompile_occurences.py ; cd .. ; RUBYOPT='-W0' bundle install; RUBYOPT='-W0' bundle exec jekyll build` (or `serve`)
