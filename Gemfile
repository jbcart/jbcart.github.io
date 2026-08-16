source "https://rubygems.org"

# Site is built by a GitHub Actions workflow (.github/workflows/pages.yml),
# not classic GitHub Pages, so we're not pinned to the github-pages gem's
# frozen Jekyll/Liquid versions.
gem "jekyll", "~> 4.3"
gem "minimal-mistakes-jekyll"

group :jekyll_plugins do
  gem "jekyll-paginate"
  gem "jekyll-sitemap"
  gem "jekyll-gist"
  gem "jekyll-feed"
  gem "jekyll-include-cache"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data
# gem and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?

# webrick is required by Jekyll's local server since it was removed from
# the Ruby standard library in Ruby 3.0.
gem "webrick", "~> 1.8"
