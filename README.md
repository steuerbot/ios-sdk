# Steuerbot iOS SDK

This Swift Package allows you to add the Steuerbot SDK to your iOS App.

## Installation

### Add the Swift Package to your Project
Add the package by selecting `File` → `Add Packages…` in Xcode’s menu bar. Search for the Steuerbot SDK using the repo's URL:

```console
https://github.com/steuerbot/ios-sdk.git
```

Then, select `Add Package`.

### Embed the Framework

Make sure `Steuerbot` is added to `Frameworks, Libraries and Embedded Content` in your apps target.


## Usage

### Basic Initialization:
```swift
import Steuerbot
...
let user = User(email: "hello@steuerbot.com", forename: "John", surname: "Doe")
let framework = SteuerbotSDK(partnerId: "your-partner-id", token: "your-user-token", user: user)

let controller = UIViewController()
controller.view = framework.getView()
self.present(controller, animated: true, completion: nil)
```

## Detailed Instructions

You can find detailed instructions in the [Wiki](https://github.com/steuerbot/ios-sdk/wiki)

## License
The contents of this repository are licensed under the [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
