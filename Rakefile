require_relative "./config/environment"
require "sinatra/activerecord/rake"
require "bundler/setup"
Bundler.require

task :console do
  require "irb"
  ARGV.clear
  IRB.start
end

ActiveRecord::Base.establish_connection(
  :adapter => "sqlite3",
  :database => "db/artists.sqlite",
)
