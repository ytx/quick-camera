# Quick Camera

Quick Camera is a MacOS utility that displays the output from any of your web cameras on your desktop. Quick Camera can be used for video conferences and presentations where you need to show an external device to your audience via the USB camera. 

Quick Camera supports mirroring (normal and reversed, both vertical and horizontal), can be rotated, resized to any size, and the window can be placed in the foreground.

You can find the app on the Mac App Store: https://itunes.apple.com/us/app/qcamera/id598853070?mt=12

License
-------
Copyright 2013-2023 Simon Guest

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.

You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the License for the specific language governing permissions and limitations under the License.

---

# Modification by ytx

## function to fit window to actual size of camera

menu "Fit to Actual Size" perform set the window size to the device's actual size that means pixel to pixel.

## save/load settings feature

menu "Save Settings" saves following values into UserDefaults,
borderless, aspectRetioFixed, mirrored, upsideDown, position, x, y, width, height and deviceName.
the values are used while the application starting.
multiple settings can be saved, these separated by using command line argument.
for example, you can have 2 sets of values.
```
"/Applications/Quick Camera.app/Contents/MacOS/Quick Camera" 1 &
"/Applications/Quick Camera.app/Contents/MacOS/Quick Camera" 2 &
```

menu "Clear Settings" clears *ALL* settings even if the argument applied.

## prefer saved or selected device
when video devices changed, prefer saved or selected device
