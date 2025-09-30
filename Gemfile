source "https://rubygems.org"
ruby "~> 3.4"

gem "jekyll", "~> 4.4"               # 4.4.1 as of Jan 2025
gem "just-the-docs"                  # latest theme

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
  gem "kramdown-parser-gfm", "~> 1.1"
  gem "jekyll-include-cache", "~> 0.2"  # optional, speeds theme includes
end

# Sass: Jekyll 4 works well with Dart Sass via sass-embedded
gem "sass-embedded", "~> 1.77"

group :development do
  gem "webrick", "~> 1.8"
end

# Windows-only extras (keep if you need them)
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?

# If you decide to run Ruby 3.4.x, and you still see CSV warnings,
# add this line to be future-proof on 3.4 where stdlib defaults changed:
# gem "csv"
