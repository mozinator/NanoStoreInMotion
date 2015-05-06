require "bundler/gem_tasks"
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'
require 'motion-cocoapods'
require 'motion-redgreen'

Motion::Project::App.setup do |app|
  app.name = 'NanoStoreDemo'
  app.redgreen_style = :full
  app.files += Dir.glob(File.join(app.project_dir, 'lib/nano_store/*.rb'))
  app.pods do
    pod 'NanoStore'
  end
end
