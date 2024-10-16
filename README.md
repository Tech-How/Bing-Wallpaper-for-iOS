# Bing Wallpaper for iOS
Explore the world, one photo at a time. 

<img src="https://raw.githubusercontent.com/Tech-How/Bing-Wallpaper-for-iOS/main/images/repo/readme/promo-3.png"/> -- <img src="https://raw.githubusercontent.com/Tech-How/Bing-Wallpaper-for-iOS/main/images/repo/readme/promo-4.png"/>

Can't decide on a wallpaper? Meet Bing Wallpaper for iOS. It exists for Windows and Android, and now Apple users can also enjoy Bing's daily images. The wallpapers change _automatically_ with the power of Shortcuts on iOS. And the first thing you'll see in the morning is a small banner with some info about the image. You can open the app to see more info and learn something new, or discover more images and test your knowledge with the daily quiz!

It's also perfectly optimized for iPad, iPhone, and iPod touch, so the focus of the image is always front and center. iPad users receive the 4K image, while iPhone and iPod users get the content-aware portrait image.

⚠️ Automatic blurring in iOS 16 can be disabled as per [this thread](https://github.com/Tech-How/Bing-Wallpaper-for-iOS/issues/2#issuecomment-1561979925).

**[Open in Shortcuts](https://www.icloud.com/shortcuts/54eec538f8e74fa39fbf240d8220fe5c)** (iOS 15.4 or later)

[Issues/Feedback Center](https://github.com/Tech-How/Bing-Wallpaper-for-iOS/issues/new/choose)

## Quick Start
Follow these steps to get the shortcut up and running.
- First, install the shortcut from the link above. (You'll go through a brief tutorial when you run it for the first time.)
- Once you've run the shortcut and completed the interactive tutorial, it's time to set up the automation.
  - Navigate to the automation tab, and tap the "+" icon.
  - Tap "Create Personal Automation".
  - Choose "Time of Day", and enter a time that works for you. (Different regions have different update times, but I use 5 AM EST for the default region.)
  - Search for the action "Text" and tap to insert it. Enter the number 0 in the box that appears.
  - Next, search for the action "Run Shortcut" and tap to insert it. Choose "Bing Wallpaper for iOS" in the box that appears.
  - Finally, tap next, and disable "Ask Before Running", and "Notify When Run".
 
[Video Tutorial](https://drive.google.com/file/d/1VqQ7kNX5cbSP8ESP7vPbpRBH8_Frod84/view)

## Add to Home Screen/Widget
For quick access, it's possible to add the shortcut to your home screen or widget.
- To add the shortcut to your home screen:
  - Tap the elipsis menu (3 dots) on the shortcut.
  - Tap the options icon in the top right-next to the close button.
  - Tap "Add to Home Screen".
  - Give it a short name so it fits on your home screen properly. (Ex. "Wallpaper")
  - Tap the icon to the left of the name, and select the image downloaded during the turorial. (Or download it [here](https://raw.githubusercontent.com/Tech-How/Bing-Wallpaper-for-iOS/main/images/shortcut/bing-icon.png).)
  - Tap "Add".
- To add the shortcut to a widget:
  - Add the Shortcuts widget to your home screen or today view.
  - Long-press on the widget, and choose "Edit".
  - Choose the same folder that your shortcut is in. You can move your shortcut by long-pressing it in the app.
  
## Changing Settings
If you'd like, you can disable some of the app's features that you don't need or want. Currently, here are the options that can be configured:
- Image Notifications
- Automatic Updates

To disable one or more of these features, open the shortcut editor by tapping on the elipsis menu (3 dots) on the shortcut. In the dictionary block underneath the release notes, delete the corresponding values that are marked with "Erase to Disable."

## Changing Language/Region
During the initial import of the shortcut, you're asked if you'd like to specify a custom language and region. The format used is "language-REGION". For example, English, United States, is en-US. And Spanish, Spain, would be es-ES. Below are references from W3Schools containing all language and country codes.
- [List of Language Codes](https://www.w3schools.com/tags/ref_language_codes.asp)
- [List of Country Codes](https://www.w3schools.com/TAGS/ref_country_codes.asp)

## Privacy Notice
The first time you run the shortcut, you will be prompted to allow access to "On my iPhone", or "On my iPad". This access is needed to remember your settings, and allow the shortcut to save data for use on next launch. Upon initial startup, a folder is created here named "Bing Wallpaper". Below is a list of all files created and how they are used:
- wpFirstRunCompleted: Remembers whether or not the tutorial was run.
- wpDisabled: Remembers if you've disabled the automation from within the shortcut.
- wpIndex: Contains the index number of the currently applied wallpaper. Used to determine what information will show on the main menu.
- wpVersion: Contains the current version of the shortcut. When read by a newer version, the post-update script will run.
- wpUpdatePush: Remembers if a push notification was sent about an update. If so, you won't be notified again unless you choose to update.

These files are stored and processed locally, and are never sent to Bing or GitHub. You can find them in the files app under "On my Device/Bing Wallpaper", and delete them at any time. However, deleting files individually may cause the shortcut to behave improperly. Deleting the entire folder will properly reset the shortcut. Wallpaper images are fetched from Microsoft Bing on each run, and are not stored here. They are only downloaded if you choose to do so from the menu.
