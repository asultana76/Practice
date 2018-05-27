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

run_context.cookbook_collection[“mycookbook”].metadata.version

Create attributes for content of the html

chef generate attribute default

attribute - Default.rb

default['my_iis']['my_msg'] = "Hello world!"

default['my_iis']['my_auth'] = "Authored by Jane Doe"



recipe - default.rb

my_msg = node['my_iis']['my_msg']

my_auth = node['my_iis']['my_auth']


content my_msg + my_auth


