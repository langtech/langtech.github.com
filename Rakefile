desc "Deploy build directory to Github pages"
task :deploy do
  puts
  puts "----Deploying branch to Github Pages."
  puts
  puts
  puts "---- Generating build using middleman."
  puts
  system "middleman build"
  system "touch build/.nojekyll"
  cd "build" do
    # puts
    # puts "---- Switching to branch development."
    # puts
    # system "git checkout master"
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
  # puts
  # puts "---- Switching to branch development."
  # puts
  # system "git checkout development"
end
task :default => :deploy