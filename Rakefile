desc "Deploy build directory to Github pages"
task :deploy do
  puts
  puts "----Deploying branch to Github Pages."
  puts
  puts
  puts "---- Generating build using middleman."
  puts
  system "middleman build"
  puts
  puts "---- Telling it to not use Jekyll."
  puts
  system "touch build/.nojekyll"
  puts
  puts "---- Copying CNAME into build."
  puts
  puts
  system "cp CNAME build/"
  cd "build" do
    puts
    puts "---- Adding build directory."
    puts
    system "git add ."
    system "git add -u"
    message = "Site updated at #{Time.now.utc}."
    puts
    puts "---- Committing: #{message}"
    puts
    system "git commit -m \"#{message}\""
    puts
    puts "---> Pushing generated website."
    puts
    system "git push -f origin master"
    puts
    puts "Github Pages deployed."
    puts
  end
end
task :default => :deploy