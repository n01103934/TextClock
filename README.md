# TextClock

# Introduction
Text Clock is an android application component that can display the current date and time as a formatted string. It uses two different formatting methods to help display the date/time in either a 24-hour format or in 12-hour format if the value does not equal zero. There is also a method that prints out the current time zone using this view. It uses a default value when a user does not specify the date information that sets the time in hours, minutes and seconds. The major purpose of my component is to give users the current time in hours, minutes and seconds as a string or character.

# History
Text Clock was first introduced and added to API level 17 in android to add another component to build a user’s apps. If you use Text Clock in your app make sure that the target compile SDK version in grade file is 17 or above. If it isn’t then android studio will give you an error like “View Required API Level 17” will be required in order for it to run. To fix the error you need to open the build.gradle(Module: app) file in your android studio project and find the minSdkVersion. Then update it to 17 or higher to be able in syncing the app successfully. The package library that my Text Clock android component was included in is android.widget.TextClock.

# Major Methods/Attributes
In order to show the current time, you need to add an xml attribute in the layout file in either 12 or 24 hour format. The attributes to use are android:format12Hour and android:format24Hour which will help specify the time using Text Clock. There is also an android:timezone attribute that can specify the time zone to use in your location such as EST, PST, etc. TextClock has inherited most of these attributes, contants, fields, methods from the two classes Text View and View. The fields for TextClock were deprecated in API level 18 so the android system just used the default value for 12 and 24 hour formats in the fields instead. It also uses public methods that returns displaying the date/time in 12 and 24 hour formats to show user the current time. Another public method returns the current time zone that a view is using when a user specifies the attribute in layout file. In addition, there are methods that sets the current date, time and time zone using TextClock. They are getFormat12Hour(), getFormat24Hour(), getTimeZone(), setFormat12Hour(), setFormat24Hour(), and setTimeZone.

# Code & Example
I have provided sample code to demonstrate an example of how to use my component TextClock. I added comments to describe how the code works, organized to get the current date/time in hours, minutes and seconds. I used many xml attributes and methods in my TextClock example to show their usage in my app for my android component. The attributes & methods I have used in my app are android:format12Hour and getFormat12Hour() to display time/date on output screen from the phone or emulator. The code is in my GitHub repository found at the following url address: https://github.com/n01103934/TextClock.


# References
I used only two sources to research my findings on the component known as TextClock. Most of my content are sourced from the open source developer android website where all the information about android is reviewed to build and innovative interactive apps for everyone. The second link is a source to show an example of how to use the TextClock component in android studio. I used something similar in my app for demonstrating an Text Clock example but I added some new and different methods to show their usage.

https://developer.android.com/reference/android/widget/TextClock
https://www.tutlane.com/tutorial/android/android-textclock-with-examples
