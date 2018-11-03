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

##### 1. Determining the device
Here you need to keep the device types in mind. This covers the screen size, CPU characteristics, resolution (DPI), storage space and   memory, and development tool environment availability.
The features in the application might have special requirements from hardware or software; this is why at the time of building app architecture you need to have the knowledge of devices that the app will support.

##### 2. Considering bandwidth
There are times when connectivity is either intermittent or not available. Your app architecture needs to be build keeping in mind the worst network scenarios. Design your caching, data access mechanism, and state management considering times of intermittent connectivity. Batch communications and choose software and hardware based on it.

##### 3. Defining user interface
You have the world and entire future ahead to show your creativity. Do not pour it all at the very first stage. Keep your user Interface as simple as possible. It has been noticed that a muddled UI becomes a major reason behind a mobile application’s failure.

##### 4. Navigation methods
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
Authentication and Authorization | **• Failing to authenticate/ authorize in occasionally connected scenarios.**<br>**• Failing to use authentication and authorization over a virtual private network (VPN).**<br>
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
## Author

<a href="https://www.linkedin.com/in/laanayabdrzak">
  <img alt="Follow me on LinkedIn"
       src="https://raw.githubusercontent.com/florent37/DaVinci/master/mobile/src/main/res/drawable-hdpi/linkedin.png" />
</a>

## Contributions
 
 Any contributions are welcome! :smile:
