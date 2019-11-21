# Uncomment the next line to define a global platform for your project
 platform :ios, '9.0'

target 'Flash Chat' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Flash Chat
pod 'Firebase','5.6.0'
pod'Firebase/Auth','5.6.0'
pod'Firebase/Database','5.6.0'
pod'SVProgressHUD'
pod'ChameleonFramework'
pod'GoogleAppMeasurement', '> 5.2.0'
pod'Firebase/Analytics','5.6.0'
pod 'Firebase/Core'
pod 'GoogleTagManager', '> 5.0'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
config.build_settings['SWIFT_VERSION'] = '3.0'
config.build_settings['MACOSX_DEPLOYMENT_TARGET'] = '10.10'
      config.build_settings['CLANG_WARN_DOCUMENTATION_COMMENTS'] = 'NO'
    end
  end
end
