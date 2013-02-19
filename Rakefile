require 'rubygems'
require './application'
require 'sequel/extensions/migration'

namespace :db do
  task :migrate => :environment do
    app = Sqrdemo::Application.new
    Sequel::Migrator.apply(app.db, 'migrate')
  end
end
