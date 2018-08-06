# UberEATS Reverse Engineering
This app is meant to be used as demo and show the various filters for restaurants near you. 

- :bow: any code review or suggestion are appreciated
- :fire: contribution is definitely welcomed
- :raised_hands: if you are a UI/UX designer and wants to see certain animation. Please Let me know!

The CI/CD will be implemented on Bitrise and the also the unit testing will be done on the data layer

| Stages                  | Status                          |  Hours |
| ----------------------- |:-------------------------------:| :-----:|
| Set User Location       |:ballot_box_with_check:          | 8      |
| Fetch Restaurants       |                                 |        |
| Filter Restaurants      | UI done                         |        |
| Fetch Restaurant Meals  |                                 |        |
| Show Restaurant Info    | :ballot_box_with_check:         |        |
| Filter Restaurant Meals | :ballot_box_with_check:         |        |
| Order Meal              |                                 |        |
| Order Payment           |                                 |        |
| Order Tracking          |                                 |        |

## Google Map Service 
- The map and the location is using Google Map Service and Google Places. Please obtain your own API token. Creating a file in the same folder where `AppDelegate.swift` with following
```swift
 import Foundation

 struct KEYS {
     static var GOOGLE_MAP_KEY: String = "YOUR_GOOGLE_ACCESS_KEY"
 }
 ```

## Go Server
- installing the golang
```
brew install go
```

- install packages
```
go get -u github.com/gorilla/mux
```
- start the server
```
cd Server
go build
./Server
```
- test the endpoint
```
curl -X GET http://localhost:8000/people
```

# Home Page
![show](https://user-images.githubusercontent.com/18454151/43353355-44e804f8-9204-11e8-9735-c321b8161d6b.gif)

# Detail View
![detail-viewgif](https://user-images.githubusercontent.com/18454151/43378304-059d4f7e-9394-11e8-85b8-7aefb9896e65.gif)
