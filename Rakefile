desc "Deploy the website"
task :deploy do
  dir = File.dirname(__FILE__)
  print "Deploying contents of #{dir}/src/site/ to s3://pnwscala.org"
  system "s3cmd sync #{dir}/src/site/ s3://pnwscala.org"
end

task :default => 'deploy'
