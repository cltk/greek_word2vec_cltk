These models were made with the following CLTK code (v0.1.28).

``` python
from cltk.vector.word2vec import make_model

filepath = os.path.expanduser('~/greek_word2vec_cltk/greek_s100_w30_min5_sg.model')
make_model('tlg', lemmatize=False, rm_stops=True, size=100, window=30, min_count=5, workers=4, sg=0, save_path=filepath)

filepath = os.path.expanduser('~/greek_word2vec_cltk/greek_s100_w30_min5_sg_lemmed.model')
make_model('tlg', lemmatize=True, rm_stops=True, size=100, window=30, min_count=5, workers=4, sg=0, save_path=filepath)
```
