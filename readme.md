# Development

``. ./run.sh`` to run site for english amassing.

``cd mkdocs-material && mkdocs serve`` to run the example docs site. You may refer to example docs site to learn more about how to write this doc.

# Deploy

``
mkdocs build && touch site/.nojekyll && git commit -m \"Deploy docs to gh-pages\" && git subtree push --prefix site origin gh-pages
``