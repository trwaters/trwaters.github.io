# Tim Waters' Home Page

This is the code for [my personal website](https://trwaters.github.io) - a clone of [Robert Spurlin's fork](https://github.com/robertspurlin/robertspurlin.github.io) of [Yevgeniy Brikman's Home Page](https://www.ybrikman.com).  I have not deleted the blog, only de-activated the link to it in `_config.yml`; in fact, I added Mathjax to it, as who knows, I may have the urge to blog soon (after all, it's May 2020 right now and I'm working from home during the pandemic). 

## How to make this site your own at yourusername.github.io 

### Option 1: by forking this site 

1. Fork this site
1. Rename the repo to myusername.github.io
1. Change `trwaters` in `_config.yml` to your username and update the twitter handle, etc.

### Option 2: by first cloning a local build of this site, editing on your PC, and then pushing that

1. Use Git to clone this repo.
1. Make sure you have [Jekyll](http://jekyllrb.com/docs/installation/) installed.
1. Just the first time: `bundle install`.
1. Delete `_config.yml` and then rename `_config.yml.local` to `_config.yml`.  
1. To build the local site and serve it: `bundle exec jekyll serve`.
1. To test: in a browser, go to `http://localhost:4000`.
1. Edit to your liking.
1. Make a new repo on github named myusername.github.io without a Readme.md or .gitignore
1. Push your local build.
1. Rename `_config.yml` to something different like `_config.yml.local` and then rename `_config.yml.github` to `_config.yml`.    Incorporate any necessary sylistic changes from `_config.yml.local` to `_config.yml` without altering the required github      settings.  Similarly rename `Gemfile` to `Gemfile.local` and `Gemfile.github` to `Gemfile`.
1. Under the `Branches` tab in Settings, make sure the repo is set to `master` (not gh-pages).  Finally, in the GitHub Pages section of the Options tab of Settings, make sure the site built correctly (and if not, debug).
1. In your local repo, issue ```git update-index --assume-unchanged Gemfile``` and ```git update-index --assume-unchanged _config.ylm``` to not sync these files once all setup.  

See the [Jekyll](http://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/)
documentation for more info.

## Technologies

1. Built with [Jekyll](http://jekyllrb.com/). This website is completely static
   and I use basic HTML or Markdown for everything.
1. Hosted on [GitHub Pages](https://pages.github.com/). I'm using the
   [GitHub Pages Gem](https://help.github.com/articles/using-jekyll-with-pages/)
   and only Jekyll plugins that are
   [available on GitHub Pages](https://help.github.com/articles/repository-metadata-on-github-pages/).
1. Free SSL and CDN provided by [CloudFlare](https://www.cloudflare.com/).    
1. The design is loosely based on [Kasper](https://github.com/rosario/kasper),
   [Pixyll](http://pixyll.com/), and [Medium](https://medium.com/).
1. Uses [Basscss](http://www.basscss.com/), [Sass](http://sass-lang.com/),
   [Font Awesome Icons](http://fortawesome.github.io/Font-Awesome/icons/),
   [Hint.css](http://kushagragour.in/lab/hint/),and
   [Google Fonts](https://www.google.com/fonts) for styling.
1. Uses [jQuery](https://jquery.com/), [lazySizes](http://afarkas.github.io/lazysizes/),
   and [responsive-nav.js](http://responsive-nav.com/) for behavior.
1. Uses [Google Analytics](http://www.google.com/analytics/) for monitoring and
   metrics.

## License

This code is released under the MIT License. See LICENSE.txt.
