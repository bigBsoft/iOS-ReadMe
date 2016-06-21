#<Project Name>
===========================
<Project> is an iOS app

##Swift Style Guide

Code follows [Raywenderlich][RW] style guide.
Lint are used before sending pull request. [SwiftLint][SL] autocorrect is used along with [Tailor][TL].

##Dependencies

Thrid party framewoks and Library are managed using Cocoapods.

### Pods used 

### Carthage used

github "SwiftyJSON/SwiftyJSON"
github "Alamofire/Alamofire"

###Version Management

Build Number willl increased for each iTunes submission
each version will have build no starting frmo 1000

##Folder Structure and Architecture

- Each `Module` Will have its own folder. eg - 
- Onboarding
- Profile
- Generic View, Data Model, Helper etc each will have its own folder
- `SupportingFiles` folder will have
- Bridging-Header.h
- Frameworks (Folder for 3rd paty code which does not have Cocoapods) 
- AppDelegate.swift
- LaunchScreen.storyboard
- Info.plist

[RW]: https://github.com/raywenderlich/swift-style-guide
[SL]: https://github.com/realm/SwiftLint
[TL]: https://tailor.sh/
