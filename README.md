# Practice
For my own sanity

https://github.com/anniehedgpeth/chef-certification-study-guides/blob/master/local-cookbook-development/local-cookbook-development-study-guide.md

Commands to upload cookbooks to the github repository

chef generate cookbook example_cookbook

cd example_cookbook

Chef generate attribute default

delivery init 

git init

git add README.md

git commit -m "Initial Commit"

remote add origin https://github.com/asultana76/cookbookname.git

push -u origin master

keyin username and password when prompted

How to reference metadata information in recipe

metadata_file = ARGV.first || 'metadata.rb'

metadata = Chef::Cookbook::Metadata.new

metadata.from_file(metadata_file)


puts "#{metadata.name} #{metadata.version}"


metadata.dependencies.each do |cookbook, version|

puts "#{cookbook} #{version}"
