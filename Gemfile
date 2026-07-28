# frozen_string_literal: true

source "https://rubygems.org"

gem "github-pages", "~> 232", group: :jekyll_plugins
gem "jekyll-figure"
gem "rake", ">= 0.9.2"
gem "webrick", "~> 1.7"  # Needed for Ruby ≥ 3.0

# 👇 Add this to support Ruby ≥ 3.1+ where csv is no longer bundled
gem "csv", "~> 3.2"
gem "bigdecimal", "~> 3.1"
gem "zeitwerk", "< 2.7"
# The github-pages gem pins Jekyll 3.9 / Liquid 4.0.3, which calls the removed
# String#tainted? and therefore only runs on Ruby 3.1.x (not 3.2+). Constrain the
# local Ruby to 3.1.x so `bundle` fails fast with a clear message on newer Rubies.
ruby "~> 3.1.0"
