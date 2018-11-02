# Presentation

Just like software, this document will rot unless we take care of it. We encourage everyone to help us on that – just open an issue or send a pull request!

Interested in mobile platforms? Our Best Practices in [Android Development](https://github.com/laanayabdrzak/MobileArchitecture/android-best-practices) and [iOS Development](https://github.com/laanayabdrzak/MobileArchitecture/ios-best-practices) Best Practices documents have got you covered.


## Contents

If you are looking for something specific, you can jump right into the relevant section from here.

1. [Getting Started](#getting-started)
1. [Architecture](#architecture)
1. [Design Considerations](#design-considerations)
1. [Stores](#stores)
1. [Assets](#assets)
1. [Coding Style](#coding-style)
1. [Security](#security)
1. [Diagnostics](#diagnostics)
1. [Analytics](#analytics)
1. [Building](#building)
1. [Deployment](#deployment)
1. [License](#license)

## Getting started

The primary reason behind this is the loopholes in mobile app architecture & mobile app development process.

## Architecture

mobile app architecture is a set of patterns and techniques which are required to be followed in order to build a fully structured mobile application. The techniques and patterns are formulated keeping the vendor requirement and industry standards in mind.
![Mobile Architecture](https://github.com/laanayabdrzak/MobileArchitecture/images/mobile-app-architectures.jpg)

While building better app architecture is vital for any business, not many appreneurs succeed in doing it. Here are few considerations you need to check at the time of building mobile app architecture:
##### The various elements of an app’s architecture

A mobile application will normally be structured as a multi-layered application consisting of user experience, business, and data layers. When developing a mobile application, you may choose to develop a thin Web-based client or a rich client. If you are building a rich client, the business and data services layers are likely to be located on the device itself. If you are building a thin client, the business and data layers will be located on the server. Figure 1 illustrates common rich client mobile application architecture with components grouped by areas of concern.

## Design Considerations

**1. Determining the device**
  Here you need to keep the device types in mind. This covers the screen size, CPU characteristics, resolution (DPI), storage space and   memory, and development tool environment availability.
The features in the application might have special requirements from hardware or software; this is why at the time of building app architecture you need to have the knowledge of devices that the app will support.

**2. Considering bandwidth**
There are times when connectivity is either intermittent or not available. Your app architecture needs to be build keeping in mind the worst network scenarios. Design your caching, data access mechanism, and state management considering times of intermittent connectivity. Batch communications and choose software and hardware based on it.

**3. Defining user interface**
You have the world and entire future ahead to show your creativity. Do not pour it all at the very first stage. Keep your user Interface as simple as possible. It has been noticed that a muddled UI becomes a major reason behind a mobile application’s failure.

**4. Navigation methods**
This one again comes on the design front. However, it requires expertise in both front and back end. There are numerous ways to navigate through app features, it is important for you to analyze which one’s good for your mobile application. The list includes:

Single view
Stacked navigation Bar
Tab controller
Scroll views
Search driven
Model controller
Gesture-based
Understand your customers and the app requirement and according chose the navigation method as it directly impacts your user experience.

## Author

<a href="https://www.linkedin.com/in/laanayabdrzak">
  <img alt="Follow me on LinkedIn"
       src="https://raw.githubusercontent.com/florent37/DaVinci/master/mobile/src/main/res/drawable-hdpi/linkedin.png" />
</a>

## Contributions
 
 Any contributions are welcome! :smile:
