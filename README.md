#Project Name
===========================
Project is an iOS app

##Swift Style Guide

Code follows [Raywenderlich][RW] style guide.
Lint are used before sending pull request. [SwiftLint][SL] autocorrect is used along with [Tailor][TL].

##Dependencies

Thrid party framewoks and Library are managed using Cocoapods.

### Pods used 
	- pod 'SwiftyJSON'
	- pod 'Alamofire'

### Carthage used

	- github "SwiftyJSON/SwiftyJSON"
	- github "Alamofire/Alamofire"

###Version Management

* Build Number willl increased for each iTunes submission
* App version will only increase on app submiting to App Store
* Each version will have build no starting from 1000

##Folder Structure and Architecture

- Each `Module` Will have its own folder. eg - 
	- Splash
	- Onboarding
	- Profile
- Constants, Generic View, Data Model, Helper etc each will have its own folder
- `SupportingFiles` folder will have
	- Bridging-Header.h
	- Frameworks (Folder for 3rd paty code which does not have Cocoapods) 
	- AppDelegate.swift
	- LaunchScreen.storyboard
	- Info.plist

##Git

- `dev` will be the semi-stable branch with `tag` on each stable merge. This is the branch from where IPA should be published to iTunes Test Flight
- `master` will have code that are fully stable with `release` on each merge. App store publishing should be done from this branch only.
- Each branch should start with two or three letter Project Name, MileStone
 `<Project-Name>-<Mile-Stone>-<Module-Name>` 
	-  BG-M5-Login
- Git commit should have multiline comments, where first line comment should start with tag like 
	- [FIXED] 
	- [ADDED]
	- [UPDATED]
	- [TEST]

[RW]: https://github.com/raywenderlich/swift-style-guide
[SL]: https://github.com/realm/SwiftLint
[TL]: https://tailor.sh/
[GF]: https://www.atlassian.com/git/tutorials/comparing-workflows