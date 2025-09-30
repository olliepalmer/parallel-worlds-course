source "https://rubygems.org"
ruby "3.3.6"

# Core
gem "jekyll", "~> 4.3"

# Theme
gem "just-the-docs"         # keep your existing theme

# Plugins used at build time
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"   # latest compatible
  gem "kramdown-parser-gfm", "~> 1.1"
  gem "jekyll-include-cache", "~> 0.2"  # improves just-the-docs perf; optional but recommended
end

# Local dev only (doesn't affect Netlify)
group :development do
  gem "webrick", "~> 1.8"
end

# Windows-only bits (leave as-is if you do Windows dev)
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?
gem "csv"
gem "logger"
