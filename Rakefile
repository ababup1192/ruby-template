# task :default => [:init, :test]

task :init do
  system "bundle install --path vendor/bundle --without production"
end

task :test do
  Dir.glob('./test/*_test.rb').each { |test_file|
    system "bundle exec ruby #{test_file}"
  }
end
