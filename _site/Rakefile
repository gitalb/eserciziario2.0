# Sources:
# http://jasonseifer.com/2010/04/06/rake-tutorial
# http://elia.wordpress.com/2008/11/07/get-input-in-rake-tasks/
# http://www.layouts-the.me/rake/2011/04/23/rake_tasks_for_jekyll/

# Asking for title
def ask message
print message
STDIN.gets.chomp
end


#Create new a post
desc "Default 'rake' command creates a new post"
task "post" do
  title = ask('Title: ')
  level = ask('Level: ')
  categories = ask('Categories: ')
  filename = "#{Time.now.strftime('%Y-%m-%d')}-#{title.gsub(/\s/, '_').downcase}.markdown"
  path = File.join("_posts", filename)
  if File.exist? path; raise RuntimeError.new("File exists #{path}"); end
  File.open(path, 'w') do |file|
    file.write <<-EOS
---
layout: post
title: \"#{title}\"
date: #{Time.now.strftime('%Y-%m-%d %k:%M:%S')} +0100
categories: [#{categories}]
level: #{level}
---
EOS
end

# invoke Textmate to edit file
# sh "mate #{path}"

    end

#Create new a category
desc "Creates a new category"
task "category" do
  title = ask('Category title (i.e. Args): ')
  category = ask('Category name (i.e. args): ')
  description = ask('Category description (i.e. Esercizi sugli argomenti da linea di comando.): ')
  filename = "index.markdown"
  path = File.join(category, filename)
  path = File.join("categories", path)
  mkdir_p path.pathmap("%d")
  if File.exist? path; raise RuntimeError.new("File exists #{path}"); end
  File.open(path, 'w') do |file|
    file.write <<-EOS
---
layout: categories
title: \"#{title}\"
category: #{category}
description: #{description}
---
EOS
end

# invoke Textmate to edit file
# sh "mate #{path}"

    end