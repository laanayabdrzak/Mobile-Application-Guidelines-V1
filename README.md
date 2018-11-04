# Presentation

Just like software, this document will rot unless we take care of it. We encourage everyone to help us on that – just open an issue or send a pull request!

Interested in mobile platforms? Our Best Practices in [Android Development](https://github.com/laanayabdrzak/Mobile-Application-Guidelines-V1/blob/master/android-best-practices.md) and [iOS Development](https://github.com/laanayabdrzak/Mobile-Application-Guidelines-V1/blob/master/ios-best-practices.md) Best Practices documents have got you covered.


## Contents

If you are looking for something specific, you can jump right into the relevant section from here.

1. [Getting Started](#getting-started)
1. [Architecture](#architecture)
1. [Design Considerations](#design-considerations)
1. [Common Issues](#common-issues)
1. [Key Design Principles](#key-design-principles)
1. [Assets](#assets)
1. [Coding Style](#coding-style)
1. [Security](#security)
1. [Diagnostics](#diagnostics)
1. [Analytics](#analytics)
1. [Building](#building)
1. [Deployment](#deployment)


## Getting started

The primary reason behind this is the loopholes in mobile app architecture & mobile app development process.

## Architecture

Mobile app architecture is a set of patterns and techniques which are required to be followed in order to build a fully structured mobile application. The techniques and patterns are formulated keeping the vendor requirement and industry standards in mind.

   ![Mobile Architecture](https://github.com/laanayabdrzak/Mobile-Application-Guidelines-V1/blob/master/mobile-app-architectures.jpg)

**The various elements of an app’s architecture**

A mobile application will normally be structured as a multi-layered application consisting of user experience, business, and data layers. When developing a mobile application, you may choose to develop a thin Web-based client or a rich client. If you are building a rich client, the business and data services layers are likely to be located on the device itself. If you are building a thin client, the business and data layers will be located on the server. The figure above illustrates common rich client mobile application architecture with components grouped by areas of concern.

## Design Considerations

The following design guidelines provide information about different aspects you should consider when designing a mobile application. Follow these guidelines to ensure that your application meets your requirements and performs efficiently in scenarios common to mobile applications:

#### 1. Determining the device
Here you need to keep the device types in mind. This covers the screen size, CPU characteristics, resolution (DPI), storage space and   memory, and development tool environment availability.
The features in the application might have special requirements from hardware or software; this is why at the time of building app architecture you need to have the knowledge of devices that the app will support.

#### 2. Considering bandwidth
There are times when connectivity is either intermittent or not available. Your app architecture needs to be build keeping in mind the worst network scenarios. Design your caching, data access mechanism, and state management considering times of intermittent connectivity. Batch communications and choose software and hardware based on it.

#### 3. Defining user interface
You have the world and entire future ahead to show your creativity. Do not pour it all at the very first stage. Keep your user Interface as simple as possible. It has been noticed that a muddled UI becomes a major reason behind a mobile application’s failure.
User interfaces must feel natural without many distraction or the users will get frustrated and leave the app altogether. A greater part of our design philosophy involves cutting the clutter to attain the simplest form of user experience.

#### 4. Navigation methods
This one again comes on the design front. However, it requires expertise in both front and back end. There are numerous ways to navigate through app features, it is important for you to analyze which one’s good for your mobile application. The list includes:

 - Single view
 - Stacked navigation Bar
 - Tab controller
 - Scroll views
 - Search driven
 - Model controller
 - Gesture-based
 
Understand your customers and the app requirement and according chose the navigation method as it directly impacts your user experience.

##### 5. Resource constraints
Every design decision should take into account the limited CPU, memory, storage capacity, and battery life of mobile devices. **Battery life** is usually the most limiting factor in mobile devices. **Battery life** is usually the most limiting factor in mobile devices. Backlighting, reading and writing to memory, wireless connections, specialized hardware, and processor speed all have an impact on the overall power usage. 

## Common Issues
There are several common issues that you must consider as your develop your design. These issues can be categorized into specific areas of the design. The following table lists the common issues for each category where mistakes are most often made.

Category | Key issues
------------ | -------------
Authentication and Authorization | **• Failing to authenticate and authorize in occasionally connected scenarios.**<br>**• Failing to use authentication and authorization over a virtual private network (VPN).**<br>**• Failing to authenticate for all connection scenarios, such as over the air, cradled, Bluetooth, and Secure Digital (SD) cards..**
Caching | **• Caching unnecessary data on a device that has limited resources. **<br>**• Caching sensitive data in unencrypted form.** <br>**• Failing to choose an appropriate caching technology.** <br>**• Choosing inappropriate cache locations and formats.** <br>**• Relying on cached data that may no longer be available in occasionally connected scenarios.**
Communication | **• Failing to protect sensitive data over the air.**<br>**• Failing to secure Web service communication.**<br>**• Failing to secure communication over a VPN.**<br>**• Not appreciating the performance impact of communication security on limited-bandwidth connections.**<br>**• Not managing limited-bandwidth connections efficiently.**<br>**• Not managing connections to multiple network services efficiently**<br>**• Not designing to work with intermittent connectivity.**<br>**• Not designing to minimize power usage when running on battery power.**
Configuration Management | **• Failing to restore configuration state after a reset.**
Data Access | **•Failing to implement data-access mechanisms that work with intermittent connectivity.**<br>**• Not considering database access performance.**<br>**• Navigating through large datasets when not required**
Device | **• Failing to consider device heterogeneity, such as screen size and CPU power.**<br>**• Not presenting user-friendly error messages to the user.**<br>**• Failing to protect sensitive information.**<br>**• Failure to consider the processing power of the device.**
Exception Management |**• Not recovering application state after an exception.**<br>**• Revealing sensitive information to the end user.**<br>**• Not logging sufficient details about the exception.**<br>**• Using exceptions to control application flow.**
Synchronization |**• Failing to secure synchronization when communicating.**<br>**• Failing to manage synchronization over the air as opposed to cradled synchronization.**<br>**• Failing to manage synchronization interruptions.**<br>**• Failing to handle synchronization conflicts.**<br>**• Failing to consider merge replication where appropriate.**
Testing |**• Failing to appreciate debugging costs when choosing to support multiple device types.**<br>**• Failing to design with debugging in mind; for example, using emulators instead of the actual devices.**<br>**• Failing to debug in all connection scenarios.**
UI |**• Not considering that only one application can be running.**<br>**• Not designing a touch-screen or stylus-driven UI for usability.**<br>**• Not including support for multiple screen sizes and orientations.**<br>**• Not managing device reset and resume.**
Validation |**• Not validating input and data during host PC communication.**<br>**• Not validating input and data during over-the-air communication.**
                                

## Key Design Principles
When getting started with your design, bear in mind the key principles that will help you to create architecture that meets “best practices,” minimizes costs and maintenance requirements, and promotes usability and extendibility. [Read more...](https://android.jlelse.eu/android-development-the-solid-principles-3b5779b105d2)
## Assets

## Coding styles
In general they are a set of standards and guidelines which are/should be used when writing the source code for a program
#### Naming
 - Meaningful names and functions.
 - Use pronounceable names.
 - Classes and objects should have noun or noun phrase names like Customer, WikiPage, Account, and AddressParser. Avoid words like Manager, Processor, Data, or Info in the name of a class. A class name should not be a verb.
 - Methods should have verb or verb phrase names like postPayment, deletePage, or save.
 
#### Structure
 - Comments are a great way to group your methods, especially in view controllers. 
 - Use styles to avoid duplicate attributes in layout XMLs.
 - Do not make a deep hierarchy of ViewGroups
 - Organization build logic approach: **Gradle, CocoaPods, Carthage**

#### External style guides
It can however be useful to peruse the style guides of other software companies, even if some bits can be quite company-specific or opinionated.

**GitHub**: [Swift](https://github.com/github/swift-style-guide)<br>
**Ray Wenderlich**: [Swift](https://github.com/raywenderlich/swift-style-guide) 

## Security
Even in an age where we trust our portable devices with the most private data, app security remains an often-overlooked subject. Try to find a good trade-off given the nature of your data; following just a few simple rules can go a long way here. A good resource to get started is Apple's own [iOS Security Guide](https://www.apple.com/business/site/docs/iOS_Security_Guide.pdf).

#### Data Storage
If your app needs to store sensitive data, such as a username and password, an authentication token or some personal user details, you need to keep these in a location where they cannot be accessed from outside the app. Never use NSUserDefaults, other plist files on disk or Core Data for this, as they are not encrypted! In most such cases, the iOS Keychain is your friend. If you're uncomfortable working with the C APIs directly, you can use a wrapper library such as `SSKeychain` or `UICKeyChainStore`.

When storing files and passwords, be sure to set the correct protection level, and choose it conservatively. If you need access while the device is locked (e.g. for background tasks), use the "accessible after first unlock" variety. In other cases, you should probably require that the device is unlocked to access the data. Only keep sensitive data around while you need it.

#### Networking
Keep any HTTP traffic to remote servers encrypted with TLS at all times. To avoid `man-in-the-middle` attacks that intercept your encrypted traffic, you can set up certificate pinning. Popular networking libraries such as **Retrofit** and **Alamofire** support this out of the box.

#### Logging
Take extra care to set up proper log levels before releasing your app. Production builds should never log passwords, API tokens and the like, as this can easily cause them to leak to the public. On the other hand, logging the basic control flow can help you pinpoint issues that your users are experiencing.

#### User interface
When using `TextFields` for password entry, remember to set their `secureTextEntry` property to true to avoid showing the password in cleartext. You should also disable auto-correction for the password field, and clear the field whenever appropriate, such as when your app enters the background.

When this happens, it's also good practice to clear the Pasteboard to avoid passwords and other sensitive data from leaking. As iOS may take screenshots of your app for display in the app switcher, make sure to clear any sensitive data from the UI before returning from `applicationDidEnterBackground`.

## Author

<a href="https://www.linkedin.com/in/laanayabdrzak">
  <img alt="Follow me on LinkedIn"
       src="https://raw.githubusercontent.com/florent37/DaVinci/master/mobile/src/main/res/drawable-hdpi/linkedin.png" />
</a>

## Contributions
 
 Any contributions are welcome! :smile:
