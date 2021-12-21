use_frameworks!

platform :ios, '14.0'

target 'Cast_IMA_Support_iOS' do
  platform :ios, '14.0'
  pod 'google-cast-sdk'
  pod 'GoogleAds-IMA-iOS-SDK'
end

post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
  end
end
