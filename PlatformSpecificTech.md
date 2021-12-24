# Platform Specific Tech

[к оглавлению](./README.md)

## Содержание

- [User Notifications](./PlatformSpecificTech.md#user-notifications)
- [Location and Map](./PlatformSpecificTech.md#location-and-map)
- [Application Lifecycle](./PlatformSpecificTech.md#application-lifecycle)
- [Animations](./PlatformSpecificTech.md#animations)
- [Apple Developer Portal](./PlatformSpecificTech.md#apple-developer-portal)
- [Core Data/Realm](./PlatformSpecificTech.md#core-data-realm)
- [RxSwift](./PlatformSpecificTech.md#rx-swift)


## <a id="user-notifications"></a> User Notifications

## Qualified:
### 1. Knows how and when to subscribe/unsubscribe for notifications
    * ?
### 2. Knows remote notification payload and purpose of each parameter
    * ?

## Competent:
### 1. Completely understands how remote notifications flow works from front-end and back-end perspective
    * ?
### 2. Knows how to manage app badge value
    * ?
### 3. Knows when device token could be refreshed
    * ?
### 4. Knows what is silent remote notification and its purpose
    * ?

## Expert:
### 1. Has experience in PushKit. VoIP notifications specifics
    * ?
### 2. Knows how to pre-process remote notification payload before app receives it
    * ?
### 3. Knows how to customize notification appearance in Notifications Center
    * ?

## <a id="location-and-map"></a> Location and Map

## Qualified:
### 1. Knows how to determine the current location
    * ?
### 2. Knows modes of CLLocationManager
    * ?

## Competent:
### 1. Knows how to implement geocoding, reverse geocoding
    * ?
### 2. Knows how to implement geofencing
    * ?
### 3. Knows how iBeacon works
    * ?
### 4. Knows what types of accuracy exist and when to use each of them
    * ?

## Expert:
### 1. Can imagine and discuss how to denoise locations, how to detect and filter invalid locations
    * ?

## <a id="application-lifecycle"></a> Application Lifecycle

## Qualified:
### 1. Knows about app states and transitions between them
    * ?
### 2. Can name most of the methods from AppDelegate and their purposes
    * ?

## Competent:
### 1. Knows how to perform some logic blocks in the background
    * ?
### 2. Knows what background modes iOS app support and how to configure them
    * ?

## Expert:
### 1. Know how to implement application state restoration
    * ?

## <a id="animations"></a> Animations

## Qualified:
### 1.  Knows what is CALayer, its subclasses
    * ?
### 2. Basic UIView animations
    * ?
### 3. Understands layer geometry (frame, bounds, anchorPoint, position), layers hierarchy
    * ?
### 4. Knows how to animate layer properties
    * ?

## Competent:
### 1. Knows differences between Model, Presentation and Render trees (layers)
    * ?
### 2. Understands time-related parameters of animations (beginTime, timeOffset, duration, speed)
     * ?
### 3. Knows how to chain or combine multiple animations
    * ?
### 4. Knows how to use transforms (CATransform3D), helper methods for transform creations/manipulations (CATransform3DMakeScale, CATransform3DTranslate, …)
     * ?
### 5. Knows how to perform custom animated screen transitions
    * ?

## Expert:
### 1. Creates easily configured and reused in different cases animation components
    * ?
### 2. Knows how to optimize animation performance.
    * ?
### 3. Understands what kinds of animations are calculated in CPU and GPU
    * ?

## <a id="apple-developer-portal"></a> Apple Developer Portal

## Qualified:
### 1. Knows what are certificates and provision profiles
    * ?
### 2. Knows what to do if there is a task to add new device
    * ?
### 3. Understand the difference between Development and Production certificates and provision profiles
    * ?
### 4. Knows how to create a new app
    * ?

## Competent:
### 1. Knows how to generate all required keys, certificates and profiles, including ones for remote notifications
    * ?
### 2. Knows about internal/external testing on TestFlight, limitations and features
    * ?
### 3. Knows how to properly export certificates and profiles from Keychain
    * ?

## Expert:
### 1. Knows what limitations have standard Apple Developer Program (number of devices, distribution certs, ways of apps distribution for in-house testing)
    * ?
### 2. Knows what Apple Developer Enterprise Program is and what benefits it has (compared with standard Developer Program)
    * ?

## <a id="core-data-realm"></a> Core Data/Realm

## Qualified:
### 1. Knows how to setup data storage using Core Data or Realm
    * ?
### 2. CRUD operations. Data observing
    * ?
### 3. Understands NSManagedObjectContext/Realm objects concept and purpose
    * ?
### 4. Knows storage types for Core Data
    * ?

## Competent:
### 1. Knows how to perform lightweight and custom migrations
    * ?
### 2. Concurrency in Core Data and Realm - bottlenecks, solutions (thread-safety, saving/merging/refreshing)
    * ?
### 3. Can explain the concept of lazy fetching in both solutions
    * ?

## Expert:
### 1. Knows features and limitations of Core Data and Realm in comparison (encryption, inheritance, grouping, fetch optimizations, …)
    * ?

## <a id="release-success-indicators"></a> RxSwift

## Qualified:
### 1. Understands concept of subscriptions
    * ?
### 2. Knows what is disposeBag and why you need it
    * ?
### 3. Knows some RX operators
    * ?
### 4. UI binding
    * ?

## Competent:
### 1. Knows lot of RX operators
    * ?
### 2. Knows about Traits (Driver, Relays, Single,…), their differences and usecases to use them
    * ?
### 3. Understands concurrency: schedulers, subscribeOn, observeOn
    * ? 
### 4. Uses operators chaining without side effects and outside context capturing (functional way of programming)
    * ?

## Expert:
### 1. Knows how to write Reactive extensions\
    * ?
