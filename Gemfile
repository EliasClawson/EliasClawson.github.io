source "https://rubygems.org"

# Force Jekyll to use version 4.2.0
gem "jekyll", "4.2.0"

# Comment out the default theme (minima) since we're using a different theme
# gem "minima", "~> 2.5"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1", platforms: [:mingw, :x64_mingw, :mswin]
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]

gem "jekyll-remote-theme", "~> 0.4.1"
gem "jekyll-paginate"
gem "jekyll-sitemap"
gem "jekyll-archives"
gem "jekyll-toc"
gem "jekyll-include-cache"
gem "webrick"