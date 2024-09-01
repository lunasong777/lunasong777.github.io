source "https://rubygems.org"

# GitHub Pages에서 요구하는 jekyll 버전
gem "github-pages", "~> 231"

# jekyll과 관련된 플러그인 설정
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-paginate"
  gem "jekyll-sitemap"
  gem "jekyll-gist"
  gem "jekyll-algolia"
  gem "jekyll-include-cache"
  gem "jekyll-sass-converter"
end

# Windows 및 JRuby의 경우, tzinfo 및 tzinfo-data 추가
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Windows 성능 향상
gem "wdm", "~> 0.1.1", platforms: [:mingw, :x64_mingw, :mswin]

# JRuby에서 http_parser.rb의 특정 버전 사용
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
