# WinUI3Preview3_Problems_CommandBarFlyout

This repository contains two solutions with sample code demonstrating the difference in appearance of the 
AppBarButton with the Flyout on a CommandBar in both UWP and WinUI3 Preview3 Desktop.

The UWP sample code only displays the AppBarButton icon, which is expected. 

However, the WinUI3 Desktop sample code displays an additional ">" or arrow next to the AppBarButton icon, which is unexpected.

----

**Describe the bug**

We used a CommandBar with AppBarButton with a Flyout in our UWP application. However, once we switched over to WinUI3 Preview 3 Desktop, the appearance of the button changed. 

The button in the WinUI3 Preview3 application has a ">" next to the icon whereas the UWP application did not. 

See Screenshots below to compare differences.

**Steps to reproduce the bug**
1. Clone the [WinUI3 Problems CommandBarFlyout repository](https://github.com/eleanorleffler/WinUI3Preview3_Problems_CommandBarFlyout).
2. Go to the CommandBarFlyoutWinUIPreview3 folder.
3. Open the CommandBarFlyoutWinUIPreview3 solution in Visual Studio 2019 Preview.
4. Build and run with Debug x64.
5. Notice the additional ">" next to the first icon in the CommandBar on the right side of the application.

**Expected behavior**

We expect to see no difference in appearance in the UWP and WinUI3 Preview 3 Desktop CommandBar buttons. The button in the WinUI3 Preview 3 Desktop application should only be the AppBarButton icon.

Build and run the CommandBarFlyoutUWP inside the CommandBarFlyoutUWP folder to see expected behavior.

**Screenshots**


Screenshot#1 - Expected Appearance (UWP)


Screenshot#2 - Current Appearance (WinUI3 Desktop)

**Version Info**

NuGet package version: 

[Microsoft.VCRTForwarders.140 1.0.6]
[Microsoft.WinUI 3.0.0-preview3.201113.0]

Targeting:
Target: Universal Windows
Target version: Windows 10, version 1809 (10.0; Build 17763)
Min version: Windows 10, version 1803 (10.0; Build 17134)

Windows app type:
| UWP              | Win32            |
| :--------------- | :--------------- |
| 		Yes 	   |  				  |

| Windows 10 version                  | Saw the problem? |
| :--------------------------------- | :-------------------- |
| Insider Build (xxxxx)              | 						 |
| May 2020 Update (19041)            | 						 |
| November 2019 Update (18363)       | 						 |
| May 2019 Update (18362)            | 						 |
| October 2018 Update (17763)        | 			Yes			 |
| April 2018 Update (17134)          | 						 |
| Fall Creators Update (16299)       | 						 |
| Creators Update (15063)            | 						 |

| Device form factor | Saw the problem? |
| :----------------- | :--------------- |
| Desktop            | 		Yes			|
| Xbox               | 					|
| Surface Hub        | 					|
| IoT                | 					|

**Additional context**
