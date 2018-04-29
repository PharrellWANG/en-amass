# Development

``. ./run.sh`` to run site for english amassing.

``cd mkdocs-material && mkdocs serve`` to run the example docs site. You may refer to example docs site to learn more about how to write this doc.

# Deploy

``
mkdocs build && git add . && git commit -m 'udpates' && git push && git checkout gh-pages && cp -r site/* ./ && git add . && git commit -m 'site updated' && git push && git checkout master
``