DIR = File.dirname(__FILE__)

desc "Deploy the website"
task :deploy do
  print "Deploying contents of #{DIR}/src/site/ to s3://pnwscala.org"
  system "s3cmd sync #{DIR}/src/site/ s3://pnwscala.org"
end

desc "Serve the website using a local Jekyll server"
task :serve do
  print "Serving the site from #{DIR}/src/site/\n"
  print "  use ctrl-C to stop\n"
  Dir.chdir("src/site") do
    system "jekyll serve"
  end
end

task :default => 'serve'
