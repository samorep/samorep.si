source "https://rubygems.org"

# Comment out the Jekyll gem as we'll use github-pages instead
# gem "jekyll", "~> 4.3.2"
gem "minima", "~> 2.5"

# Add the github-pages gem
gem "github-pages", "~> 232", group: :jekyll_plugins

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
  gem "jekyll-seo-tag", "~> 2.8"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

