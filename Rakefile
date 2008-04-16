#
# Copyright (c) 2008 El Draper, el@eldiablo.co.uk
#
# Rakefile      Defines the Gem package specification
#
require "rubygems"
require "rake/gempackagetask"

# Define the merb-manage gem spec
spec = Gem::Specification.new do |s|
  s.name = "merb-manage"
  s.version = "0.3"
  s.author = "El Draper"
  s.email = "el@eldiablo.co.uk"
  s.homepage = "http://github.com/eldiablo/merb-manage"
  s.platform = Gem::Platform::RUBY
  s.summary = "Provides easy configuration and management of Merb applications, including multiple servers and different adapters"
  s.files = FileList["{bin,config,resources}/**/*"].to_a
  s.executables << "merb-manage-ctl"
  s.add_dependency("merb", ">= 0.9.2")
end

# Setup the package task
Rake::GemPackageTask.new(spec) do |pkg|
  pkg.need_tar = true
end