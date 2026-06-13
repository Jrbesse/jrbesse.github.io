source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins
gem "jekyll-include-cache", group: :jekyll_plugins

# Ruby 3.4+ moved these out of the default stdlib; the jekyll/github-pages
# versions pinned for GitHub Pages compatibility still expect them.
gem "csv"
gem "base64"
gem "logger"

# Windows and JRuby do not include zoneinfo files, so bundle the tzinfo-data gem
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "wdm", ">= 0.1.0" if Gem.win_platform?
end
