# SwiftUIBanner

Notification Banner built with SwiftUI.

![banner_gif](images/banner_gif_cropped.gif)

### How To Use

```swift
struct ContentView: View {
    
    @State var showBanner:Bool = true
    @State var bannerData: BannerModifier.BannerData = BannerModifier.BannerData(title: "Default Title", detail: "This is the detail text for the action you just did or whatever blah blah blah blah blah", type: .Info)
    // Also Supports Banner Types .Success, .Warning, .Error
    
    var body: some View {
        Text("Hello Trailing Closure")
            .banner(data: $bannerData, show: $showBanner)
            // Simply add the Banner to your root view, and control it using State variables.
    }
}
```

