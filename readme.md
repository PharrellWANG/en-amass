# Development

Please setup virtualenv if you don't have one. 
``
virtualenv venv -p `which python3` && pip install -r requirements.txt
``

``. ./run.sh`` from project root to run site for english amassing.

``. ./mkdocs-material-run.sh`` from ~ for example project on mbp.

Click [here](https://github.com/PharrellWANG/mkdocs-material) and run the example docs site for info
about how to write docs and use extension.

# Deploy

``
mkdocs build && git add . && git commit -m 'udpates' && git push && mkdir /tmp/en-amass && cp -r site/* /tmp/en-amass/ && git checkout gh-pages && cp -r /tmp/en-amass/* ./ && git add . && git commit -m 'site updated' && git push && git checkout master && rm -rf /tmp/en-amass
``