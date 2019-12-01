# # require_relative './config/enfironment.rb'
# # require 'sinatra/activerecord/rake'

namespace :greeting do 
desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

desc 'outputs hola to the terminal'
  task :hola do 
    puts "hola de Rake!"
  end

end

desc 'please make this truthy'
  task :console do 
    return true
    # ActiveRecord::Base.logger = Logger.new(STDOUT)
  end


namespace :db do
desc 'dunno'
  task :environment do 
    require_relative './config/environment'
  end

desc 'supposed to migrate some stuff, idk'
  task :migrate  => :environment do 
    Student.create_table
  end
end

namespace :db do

desc 'last one, eh?'
  task :seed do 
    require_relative './db/seeds.rb'
  end

end