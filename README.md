![Image](/img/github_banner.png)

### Specs
[ ![Download](https://api.bintray.com/packages/nisrulz/maven/com.github.nisrulz%3Ascreenshott/images/download.svg) ](https://bintray.com/nisrulz/maven/com.github.nisrulz%3Ascreenshott/_latestVersion)

### Badges/Featured In
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-Screenshott-brightgreen.svg?style=flat)](https://android-arsenal.com/details/1/4963#) [![AndroidDev Digest](https://img.shields.io/badge/AndroidDev%20Digest-%23125-blue.svg)](https://www.androiddevdigest.com/digest-125/)

### Show some :heart: and star the repo to support the project
[![GitHub stars](https://img.shields.io/github/stars/nisrulz/screenshott.svg?style=social&label=Star)](https://github.com/nisrulz/screenshott) [![GitHub forks](https://img.shields.io/github/forks/nisrulz/screenshott.svg?style=social&label=Fork)](https://github.com/nisrulz/screenshott/fork) [![GitHub watchers](https://img.shields.io/github/watchers/nisrulz/screenshott.svg?style=social&label=Watch)](https://github.com/nisrulz/screenshott) [![GitHub followers](https://img.shields.io/github/followers/nisrulz.svg?style=social&label=Follow)](https://github.com/nisrulz)
[![Twitter Follow](https://img.shields.io/twitter/follow/nisrulz.svg?style=social)](https://twitter.com/nisrulz)


Take a screenshot of your view layout , programmatically!

![sc1](/img/sc1.png)  ![sc2](/img/sc2.png)

# Including in your project
ScreenShott is available in the Jcenter, so getting it as simple as adding it as a dependency
```gradle
compile 'com.github.nisrulz:screenshott:{latest version}'
```
where `{latest version}` corresponds to published version in [ ![Download](https://api.bintray.com/packages/nisrulz/maven/com.github.nisrulz%3Ascreenshott/images/download.svg) ](https://bintray.com/nisrulz/maven/com.github.nisrulz%3Ascreenshott/_latestVersion)


#Usage
+ Get bitmap of screenshot

  ```java
  // View with spaces as per constraints
  Bitmap bitmap_view = ScreenShott.getInstance().takeScreenShotOfView(view);

  // RootView
  Bitmap bitmap_rootview = ScreenShott.getInstance().takeScreenShotOfRootView(view);

  // Just the View without any constraints
  Bitmap bitmap_hiddenview = ScreenShott.getInstance().takeScreenShotOfJustView(view);
  ```

+ Save the bitmap using the provided helper function

  ```java
  ScreenShott.getInstance().saveScreenshotToPicturesFolder(context, bitmap, "my_screenshot_filename");
  ```
  .. or save the bitmap with your own implementation

  > Please request the runtime permission for `android.permission.WRITE_EXTERNAL_STORAGE` to allow saving the file to external storage. The lib includes the permission, you just need to implement the runtime permission implementation code.


### Pull Requests
I welcome and encourage all pull requests. It usually will take me within 24-48 hours to respond to any issue or request. Here are some basic rules to follow to ensure timely addition of your request:
  1. Match coding style (braces, spacing, etc.) This is best achieved using `CMD`+`Option`+`L` (Reformat code) on Mac (not sure for Windows) with Android Studio defaults.
  2. If its a feature, bugfix, or anything please only change code to what you specify.
  3. Please keep PR titles easy to read and descriptive of changes, this will make them easier to merge :)
  4. Pull requests _must_ be made against `develop` branch. Any other branch (unless specified by the maintainers) will get rejected.
  5. Check for existing [issues](https://github.com/nisrulz/screenshott/issues) first, before filing an issue.
  6. Have fun!

### Created & Maintained By
[Nishant Srivastava](https://github.com/nisrulz) ([@nisrulz](https://www.twitter.com/nisrulz))

### Created & Maintained By
[Nishant Srivastava](https://github.com/nisrulz) ([@nisrulz](https://www.twitter.com/nisrulz))


> If you found this library helpful or you learned something from the source code and want to thank me, consider [buying me a cup of](https://www.paypal.me/nisrulz) :coffee:

