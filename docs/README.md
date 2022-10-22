# Webpage

## Install

```sh
# install jekyll https://jekyllrb.com/docs/installation/
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install chruby ruby-install
ruby-install ruby
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-xxx" >> ~/.zshrc
ruby -v

gem install jekyll
gem install bundler

# install dependencies using Gemfile - bundle
bundle install
```

## Run

```sh
bundle exec jekyll serve -i
```

## Publish

```sh
chmod +x publish.sh
./publish.sh
```
