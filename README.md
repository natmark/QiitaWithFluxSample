# QiitaWithFluxSample

This is a sample project that uses **Flux** and **MVVM** features.

![Qiita](./Images/Qiita.gif)

## Features

- ViewController Routing with Flux
- AccessToken management with Flux
- Items searching action with MVVM

## Flux Classes

- Application
  - ApplicationAction
  - ApplicationDispatcher
  - ApplicationStore
- Route
  - RouteAction
  - RouteDispatcher
  - RouteStore

## Structures

- RootViewController (switching currentViewController based on RouteStore's value)
  - LoginNavigationController
    - LoginTopViewController
    - LoginViewController (loading Qiita web site and authorizing user via ApplicationAction)
  - SearchNavigationController
    - SearchTopViewController (searching items from Qiita)
      - SearchTopDataSource
      - SearchTopViewModel

![structure](./Images/structure.jpeg)

## Requirements

- Swift 3.0
- Xcode 8.3
- iOS 10.0

## Libraries

- [Action](https://github.com/RxSwiftCommunity/Action) 2.2.2
- [RxSwift](https://github.com/ReactiveX/RxSwift) 3.3.1
- [APIKit](https://github.com/ishkawa/APIKit) 3.1.1
- [Himotoki](https://github.com/ikesyo/Himotoki) 3.0.1
- [Kingfisher](https://github.com/onevcat/Kingfisher) 3.6.2
- [SwiftyUserDefaults](https://github.com/radex/SwiftyUserDefaults) 3.0.0

## Special Thanks

This sample uses [Qiita API](https://qiita.com/api/v2/docs).

## Author

marty-suzuki, s1180183@gmail.com

## License

ReverseExtension is available under the MIT license. See the LICENSE file for more info.
