Minor tweaks of https://github.com/lkmvip/netflix-4K-DDplus to allow automatic
extension conversion using xcode tools. Better alternative to *Boom3D-5.1 Audio
for Netflix* which only enables HE-AAC 5.1 and is non-free.

Build
=====

```
rm -rf Netflix_Extension; xcrun safari-web-extension-converter --macos-only --no-open ./ && pushd ./Netflix_Extension && xcodebuild && popd
```

Usage
=====

Enable unsigned extentions, enable `HE-AAC` option, spatial audio will now be
available and work with your AirPods.

Automatically select best bitrate also working as expected.

All other features are unknown compatibility wise.
