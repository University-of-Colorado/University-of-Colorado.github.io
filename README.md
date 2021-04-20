This repository hosts the documentation for the University of Colorado's Github Enterprise agreement.

The philosophy here is to host this code as [Github Pages](https://docs.github.com/en/pages) so that it is in neutral territory. If needed in the future, it can obviously move elsewhere. As well, try to keep this simple, it should not be hard for almost anyone to create a page using markdown and get some documentation up quickly.

The documentation contained here makes use of [jekyll](https://jekyllrb.com) in order to be statically rendered into HTML. Github itself does all of the heavy lifting in terms of running jekyll, and there is [good documentation on using Github Pages with jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll).

However, for the truly busy, here is what you need to do in order to create a new page:
1. Copy an existing page and modify as needed paying careful attention to the metadata located between the '---' symbols, this is known as the [Front Matter](https://jekyllrb.com/docs/front-matter/)
1. Write your documentation using markdown syntax, specifically [Github Flavored Markdown](https://guides.github.com/features/mastering-markdown/#GitHub-flavored-markdown) (GFM).
1. Keep it simple, very simple, we probably do not need anything fancy on here.