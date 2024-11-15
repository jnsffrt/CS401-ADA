# Installation Guide

To install Jekyll and run the website locally.

```shell
# Install Ruby
brew install chruby ruby-install
ruby-install ruby 3.3.5

# Configure shell to automatically use chruby
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.3.5" >> ~/.zshrc # run 'chruby' to see actual version
source ~/.zshrc

# Install Jekyll
gem install jekyll
gem install jekyll bundler

# Install plugins
bundle add jekyll-remote-theme
bundle install

# Run website
bundle exec jekyll serve
```