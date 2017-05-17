# GitHub page - redirect starter

Starter repo to redirect personal site previously on GitHub pages to a new domain

How to use:

* install [Ruby](https://www.ruby-lang.org/en/downloads/) if not already installed 
* install bundle: ``gem install bundle``
* install dependencies from Gemfile: ``bundle install``
* edit ``index.md``, substituting your actual domain
* serve site to test redirect:

```console
jekyll build
bundle exec jekyll serve
```

* create [GitHub pages repo for your user](https://pages.github.com/) but do not clone
* initialize repo, stage and commit changes, add ``origin``, then push (substituting with actual username):

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:username/username.github.io
git push -u origin master
```

Note, wildcard re-directs are not possible so if you want to redirect specific articles or pages you will need to create one file like ``index.md`` for each. I'm considering a script to help with that.