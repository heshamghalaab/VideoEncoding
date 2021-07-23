[![Swift 5](https://img.shields.io/badge/Swift-5-green.svg?style=flat)](https://swift.org/)

Xcode Version 12.5.1 (12E507) 

# Video Encoding - iOS Assignment for Impressions #

The outcome of this assignment is to create an app that converts any video to the specifications outlined below. 
The output must have these specs:

| Video | Audio |
| :---     | :---     |
| H264 encoding | AAC encoding |
| 960 height, 540 width pixels, portrait mode as frame size. | Mono. Stereo input must be mixed ( L + R ) / 2 |
| 24 frames per second. | 44.1 kHz sample rate. | 
| At most one keyframe per second (can be lower). | 64 kbit per second bitrate. |
| 1.0 mbit per second bitrate. | |


### Dev Setup
```
- Just Run! 😎
```

## Dev Notes ##

### Design Pattern
- This project uses the **Model View View Model pattern**, as it has the below key values:
* **Better Separation of Concerns** The view model translates the data of the model layer into something the view layer can use. The controller is no longer responsible for this task.
* **Improved Testability** View controllers are notoriously hard to test because of their relation to the view layer. By migrating data manipulation to the view model, testing becomes much easier.
* **Transparent Communication** The responsibilities of the view controller are reduced to controlling the interaction between the view layer and the model layer, glueing both layers together. The view model provides a transparant interface to the view controller, which it uses to populate the view layer and interact with the model layer. This results in a transparant communication between the four layers of the application.

### Unit Testing
- The project uses XCTest for unit test.

