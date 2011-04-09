lib_dir = File.expand_path(File.join(File.dirname(__FILE__), 'lib'))
$:.unshift(lib_dir)
$:.uniq!

require File.join(File.dirname(__FILE__), 'lib/webfinger', 'version')
PKG_DISPLAY_NAME   = 'WebFinger'
PKG_NAME           = PKG_DISPLAY_NAME.downcase
PKG_VERSION        = WebFinger::VERSION::STRING
PKG_FILE_NAME      = "#{PKG_NAME}-#{PKG_VERSION}"

RELEASE_NAME       = "REL #{PKG_VERSION}"

PKG_AUTHOR         = 'Bob Aman'
PKG_AUTHOR_EMAIL   = 'bob@sporkmonger.com'
PKG_HOMEPAGE       = 'http://code.google.com/p/ruby-webfinger/'
PKG_SUMMARY        = 'An implementation of the WebFinger protocol for Ruby.'
PKG_DESCRIPTION    = <<-TEXT
An implementation of the WebFinger protocol for Ruby.
TEXT
begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = PKG_NAME
    gem.summary = PKG_SUMMARY
    gem.description = PKG_DESCRIPTION
    gem.email = PKG_AUTHOR_EMAIL 
    gem.homepage = PKG_HOMEPAGE
    gem.authors = [PKG_AUTHOR]
    gem.add_development_dependency "rspec"
    gem.version = '0.1'
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install   jeweler"
end

