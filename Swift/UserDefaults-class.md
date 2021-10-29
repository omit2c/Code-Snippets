# User Defaults in Swift

## Code

```swift
class Example : ObservableObject
{
    @Published var exampleInt : Int
    {
        didSet
        {
            UserDefaults.standard.set(coins, forKey: "example_key")
        }
    }
    
    init()
    {
        self.exampleInt = UserDefaults.standard.object(forKey: "example_key") as? Int ?? 0
    }
}
```

## Description

This is a simple UserDefaults class in Swift, which can be used to store variables on the device, to maintain information after restarting the app.

Find more information about UserDefaults on the [Apple Developer Documentation](https://developer.apple.com/documentation/foundation/userdefaults).


#### Version
1.0

Tested on: (Enter your system here.)

## Comments

Comments from other people on this code.