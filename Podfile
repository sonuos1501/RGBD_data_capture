# Uncomment the next line to define a global platform for your project
platform :ios, '13.4'
use_frameworks!

target 'TrueDepthStreamer' do
  pod 'Alamofire', '~> 5.6'
  pod 'Firebase/Analytics'
end



post_install do |installer|
  installer.generated_projects.each do |project|
    project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.4'
      end
    end
  end
end
