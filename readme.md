# Development

Please setup virtualenv if you don't have one. 
``
virtualenv venv -p `which python3` && pip install -r requirements.txt
``

``. ./run.sh`` to run site for english amassing.

Click [here](https://github.com/PharrellWANG/mkdocs-material) and run the example docs site for info 
about how to write docs and use extension.

# Deploy

``
mkdocs build && git add . && git commit -m 'udpates' && git push && git checkout gh-pages && cp -r site/* ./ && git add . && git commit -m 'site updated' && git push && git checkout master
``