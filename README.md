# Ionic-sidemenu-animation-bug [iOS]

**Issue available at** [ionic-team/ionic#21186](https://github.com/ionic-team/ionic/issues/21186)

**Current behavior:**  
When the `ion-content` doesn't have the `fullscreen` attribute set to `true`, the side menu closes itself instantly without any animation if the iOS device has the low power mode enabled.  

See the attached gif below. (bug occurs right after I enable the low power mode)

**GIF steps:**  
- Going from `First` to `Second` (closing menu animation ✅)
- Going from `Second` to `First` (closing menu animation ✅)
- Enabling Low Power Mode
- Going from `First` to `Second` (no closing menu animation ❌)


![](demo.gif)  

**Expected behavior:**  
The side menu should smoothly close itself, having the low power mode enabled or not.

**Other information:**  
iPhone X running iOS `13.2.2`.  

Works fine on iOS if the low power mode is disabled.  
Works fine either way on Android/Browser.
