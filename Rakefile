desc "Deploy build directory to Github pages"
task :deploy do
  puts "Generating build using middleman."
  system "middleman build"
  puts "Deploying branch to Github Pages."
  system "touch build/.nojekyll"
  cd "build" do
    system "git add ."
    system "git add -u"
    message = "Site updated at #{Time.now.utc}."
    puts "Committing: #{message}"
    system "git commit -m \"#{message}\""
    puts "Pushing generated website."
    system "git push origin master"
    puts "Github Pages deployed."
  end
end
task :default => :deploy