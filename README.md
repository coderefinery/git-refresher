# A refresher on Git

- [Credit and license](https://coderefinery.github.io/git-intro/license/)

The first Git lesson taught during CodeRefinery workshops assumes some previous
experience with Git. This short lesson goes through the necessary 
installation and configuration steps, and also covers some of the very basics of Git 
which are helpful to know before the workshop starts.

## Local development

The following Gemfile will permit you to run jekyll locally

```
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
gem 'github-linguist'
gem 'rouge', '~>1.11.1'
```

Write it as Gemfile under the repository root.

```shell
$ export GEM_HOME=$HOME/.gem
$ export PATH=$PATH:$HOME/.gem/bin
$ bundler install
$ bundle exec jekyll serve
```
