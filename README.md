# opencv-contrib-ios (4.6.0) [![Status](https://github.com/yaabukwa/opencv-contrib-ios/actions/workflows/ios.yml/badge.svg)](https://github.com/yaabukwa/opencv-contrib-ios/actions/workflows/ios.yml)

opencv-contrib-ios provides iOS xcframework with x64, arm64 precompiled binaries for device and simulator. 
It also provides podspec that can be used to seamlessly integrat opencv/contrib libraries in your application.


## How is it built

This project relies on GitHub workflows to build the packages. Artifacts generated by [Actions](https://github.com/yaabukwa/opencv-contrib-ios/actions) 
are then used in [Releases](https://github.com/yaabukwa/opencv-contrib-ios/releases). Each release should show the compilation flags that were used to 
build that specific release.

## Installation in your project

1. Make sure you have `cocoapods` installed.
```
sudo gem install cocoapods
```

2. In your `Podfile`, add the following:
```
  # Pods for OpenCV-contrib
  pod 'opencv-contrib', :podspec => 'https://github.com/yaabukwa/opencv-contrib-ios/releases/download/v1.0.0/opencv_contrib.podspec'
```

3. Run `pod install`

4. Open your `xcworkspace` file.
```
open <project_name>.xcworkspace
```
