source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '2.6.3'

gem 'rails', '~> 6.0.0.rc1'
gem 'puma', '~> 4.3'
gem 'bootsnap', '>= 1.1.0', require: false
gem 'hirb'                # コンソール出力結果を表にする
gem 'hirb-unicode'        # コンソール文字の表示を補正する
gem 'knock', '~> 2.1.1'   # JWT認証機構
gem 'bcrypt', '~> 3.1.11' # password暗号化
gem 'aws-ses', '~> 0.6'   # 本番環境 mailer

group :development, :test do
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
  gem 'dotenv-rails', '~> 2.5.0', require: 'dotenv/rails-now' # 環境変数の管理
  gem 'pry-byebug'             # binding.pry
  gem 'sqlite3', '~> 1.4'      # development DB
end

group :development do
  gem 'listen', '>= 3.0.5', '< 3.2'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
end

group :test do
  gem 'minitest-reporters', '~> 1.1.9'  # test色付け
end

group :production do
  gem 'pg', '~> 0.18.4' # heroku DB
end


# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
