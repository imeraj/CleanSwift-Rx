use_frameworks!

target 'CleanStore' do
	pod 'RxSwift', '~> 4.0'
    pod 'RxCocoa', '~> 4.0'
	pod 'SwiftLint', '0.23.1'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['CONFIGURATION_BUILD_DIR'] = '$PODS_CONFIGURATION_BUILD_DIR'
    end
  end
end
