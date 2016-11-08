# Sketch-iOS-Library
Most Sketch resources aren’t accurate and don’t share how they go the specs they’re providing. I’ve decided to find out how something looks/works in Xcode and do the best to replicate it. Even further, I share how I ended up with my result so you can take what I know and look into it further if you’re interested.

## UIFontTextStyle

![uifonttextstyles](https://cloud.githubusercontent.com/assets/3231370/20086065/77bf1428-a53b-11e6-99e7-7600cc96e0ea.png)

Apple’s system fonts are designed for legibility and provide a variety of sizes which automatically react to accessibility features. You can read more about why it’s best to use system fonts on the [iOS Human Interface Guidelines](https://developer.apple.com/ios/human-interface-guidelines/visual-design/typography/).

**Usage**

1. Open `UIFontTextStyle.sketch`
2. Copy & Paste artboard into Sketch document
3. Assign texts to a system style

**Process**

Apple provides the name of ten [text styles](https://developer.apple.com/reference/uikit/uifonttextstyle). Since we design with the default (large) dynamic type size, I decided it’d make sense to get the specs for these.

1. I made a list of these ten styles:

`Title1` `Title2` `Title3` `Headline` `Subhead` `Body` `Footnote` `Caption1` `Caption2` `Callout`

2. Printed the specs in Xcode, for example:

`UIFontTextStyle(_rawValue: UICTFontTextStyleTitle1): .SFUIDisplay-Light, 28`

3. Changed the tracking to what [designcode.io](https://designcode.io/cloud/chapter1/iOS-Tracking.jpg) recommends.

## UIBlurEffectStyle
Apple doesn’t share any specs for the three types of blurs they provide us.
