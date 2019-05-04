# Development Environment Setup

## Setting up locally with Jekyll for Windows
- Check if Ruby 2.1.0 or higher installed
```bash
$ ruby --version
> ruby 2.X.X
```
- If you don't have Ruby installed, [install Ruby 2.1.0 or higher](https://www.ruby-lang.org/en/downloads/)

- Install Bundler:
```bash
$ gem install bundler
# Installs the Bundler gem
```
- Install Jekyll and other dependencies from the GitHub Pages gem:
```bash
$ bundle install
> Fetching gem metadata from https://rubygems.org/............
> Fetching version metadata from https://rubygems.org/...
> Fetching dependency metadata from https://rubygems.org/..
> Resolving dependencies...
```
- Run your Jekyll site locally:
```bash
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
- Preview your local Jekyll site in your web browser at `http://localhost:4000`


[Tech Blog](techblog/Table-of-Contents.md)