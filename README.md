# gdx-showcase

This repo is a community effort to try to bring the libGDX site up to date and make it representative of what libGDX is capable of. The deployed page can be found **[here](https://crykn.github.io/gdx-showcase/).**

## Collaborating
If you want to collaborate, you first need to clone this repo.

### How do gh-pages work?
This page is a [Jekyll](https://jekyllrb.com/docs/github-pages/) blog, hosted via GitHub Pages. All pages and posts  need to have a YAML frontmatter for example this one:

```
layout: page
title: "Super Nice Page Title"
permalink: /best_url_path_4_ever/
```

after that, everything can be written in **markdown**. Github offers a very nice explanation on how one can add posts and pages: https://docs.github.com/en/github/working-with-github-pages/adding-content-to-your-github-pages-site-using-jekyll

The minimal mistakes theme, that is used here, also supports some nice features ([galleries](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#gallery), [header images](https://mmistakes.github.io/minimal-mistakes/docs/layouts/#header-overlay), [tables of content](https://mmistakes.github.io/minimal-mistakes/docs/layouts/#table-of-contents)), which are detailed here: https://mmistakes.github.io/minimal-mistakes/docs/quick-sb


### Deploy locally
To test your changes locally, you can deploy jekyll on your machine:
1. Install a full [Ruby development environment](https://jekyllrb.com/docs/installation/).
2. Install Jekyll and [bundler](https://jekyllrb.com/docs/ruby-101/#bundler) [gems](https://jekyllrb.com/docs/ruby-101/#gems):

```
gem install jekyll bundler
```

3. In your working directory, install the other dependencies of the gemfile:

```
bundle install
```

4. Run Jekyll locally:

```
$ bundle exec jekyll serve
> Configuration file: /Users/octocat/my-site/_config.yml
>            Source: /Users/octocat/my-site
>       Destination: /Users/octocat/my-site/_site
> Incremental build: disabled. Enable with --incremental
>      Generating...
>                    done in 0.309 seconds.
> Auto-regeneration: enabled for '/Users/octocat/my-site'
> Configuration file: /Users/octocat/my-site/_config.yml
>    Server address: http://127.0.0.1:4000/
>  Server running... press ctrl-c to stop.
```

5. Preview your local site at: [http://localhost:4000](http://localhost:4000)
