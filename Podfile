# Uncomment the next line to define a global platform for your project
workspace 'GooglePodsSwizzle'

# Comment the next line if you're not using Swift and don't want to use dynamic frameworks
use_frameworks!
pod 'CodableAlamofire'
pod 'SwiftDate'
pod 'SwiftLocation', :git => 'https://github.com/cyupa/SwiftLocation.git'

target 'GooglePodsSwizzle' do
  use_frameworks!
  platform :ios, '10.0'
  # Pods for GooglePodsSwizzle
  inherit! :complete
  pod 'AlamofireNetworkActivityIndicator'
  pod 'RxSwift'
  pod 'RxCocoa'
  pod 'RxRealmDataSources'
  pod 'RxOptional'
  pod 'DynamicColor'
  pod 'FirebaseCore'
  pod 'FirebaseAuth'
  pod 'FirebaseFirestore'
  pod 'FirebaseMessaging'
  pod 'Firebase/Performance'
  pod 'Firebase/AdMob'
  pod 'Firebase/DynamicLinks'
  pod 'SwiftLint'
  pod 'GSKStretchyHeaderView'
  pod 'Hero'
  pod 'PMAlertController'
  pod 'RealmSwift'
  pod 'RxRealm'
  pod 'ObjectMapper+Realm'
  pod 'ObjectMapperAdditions/Core'
  pod 'ObjectMapperAdditions/Realm'
  pod 'BezierPathLength', :git => 'https://github.com/cyupa/bezierpath-length.git'
  pod 'Solar'
  pod 'Fabric'
  pod 'Crashlytics'
  pod 'SwiftyStoreKit'
  pod 'UPCarouselFlowLayout', :git => 'https://github.com/cyupa/UPCarouselFlowLayout.git'
  pod 'CHIPageControl/Aleppo'

  target 'GooglePodsSwizzleTests' do
    platform :ios, '10.0'
    inherit! :complete
    # Pods for testing
    pod 'RxBlocking'
    pod 'RxTest'
    pod 'Mockingjay'
  end

  target 'GooglePodsSwizzleUITests' do
    platform :ios, '10.0'
    inherit! :complete
    # Pods for UI Testing
    pod 'RxBlocking'
    pod 'RxTest'
    pod 'Mockingjay'
  end
end

target 'GooglePodsSwizzleIntents' do
  use_frameworks!
  platform :ios, '10.0'
  inherit! :complete
end

target 'GooglePodsSwizzleIntentsUI' do
  use_frameworks!
  platform :ios, '10.0'
  inherit! :complete
end

target 'GooglePodsSwizzleWatch' do
  use_frameworks!
  platform :watchos, '3.0'
  inherit! :complete
end

target 'GooglePodsSwizzleWatchExtension' do
  use_frameworks!
  platform :watchos, '3.0'
  inherit! :complete
  pod 'YOChartImageKit', :git => 'https://github.com/cyupa/YOChartImageKit.git'
end

target 'GooglePodsSwizzleToday' do
  use_frameworks!
  platform :ios, '10.0'
  inherit! :complete
  pod 'FirebaseCore'
  pod 'Fabric'
  pod 'Crashlytics'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '4.0'
    end
  end
end
