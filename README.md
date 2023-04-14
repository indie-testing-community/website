# Indie Testing Community GH Pages Repository
This is the [GitHub Pages](https://pages.github.com/) repository for the [Indie Testing Community](https://www.indie-testing.community/) website, powered by [Jekyll](https://jekyllrb.com/) and the [Cayman](https://github.com/pages-themes/cayman) GitHub Pages theme.

## Adding new pages

See the [GitHub Pages documentation](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll) to understand how to add new pages to the site.

## Customising the theme/templates

See the [Cayman theme documentation](https://github.com/pages-themes/cayman#customizing) for instructions on editing the templates, styling and config. See also:
* [Adding a theme to your GitHub Pages site using Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll) - GitHub Pages documentation
* [Themes - Overriding Theme Defaults](https://jekyllrb.com/docs/themes/#overriding-theme-defaults) - Jekyll documentation.

## Building locally

First, ensure that you have a recent version of Ruby installed locally. 

On a Mac, you can install [rbenv](https://github.com/rbenv/rbenv) using [Homebrew](https://brew.sh/) and install a sensible version of Ruby globally or within this directory:
```
brew install rbenv 

rbenv init # follow the instructions to add rbenv to your shell

rbenv global 3.1.4  # set the default Ruby version for this machine
# or:
rbenv local 3.1.4   # after navigating this repository, run this command to set the Ruby version for just this project
```

If any of these commands don't work as they should, you may need to quit and re-open your terminal app/tab before trying again.

Once you have a sensible Ruby environment up and running, run these two commands to install dependencies:
```
gem install bundler
bundle install
```

Finally, run this command to generate the static site and serve it locally at [localhost:4000](http://localhost:4000/):
```
bundle exec jekyll serve
```

As you edit files and save them, the static site will automatically rebuild.

When committing changes, it's probably not necessary to include the generate `Gemfile.lock`, but we can do so in future if needed.