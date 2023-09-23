# **ColorMaker**

A fun, quick project led by Hector Perez on his Udemy course: *.NET MAUI course with Visual Studio 2022 creating PROJECTS*

The XAML is comprised of a Grid container, which holds a stack layout that contains labels and sliders that display the amount of red, green, and blue being added into a HEX color creator. 
These sliders receive their power from the codebehind, enabling them to combine together to create HEX values by manipulating the slider values.
Below the sliders is a random button, that generates a random HEX color, and then an image that, when clicked, copies the HEX value to the user's clipboard.

The codebehind is managed by way of a few methods:
- SetColor() assigns the HEX value to the lblHex label to display the value for the user, and changes the container and btnRandom background colors to the selected color
- btnRandom_Clicked() invokes the Random class to create 3 random RGB values, and then assigns those values to the sliders
- ImageButton_Clicked() puts the CommunityToolKit.Maui Nuget package to use, calling Toast.Make() from CommunityToolkit.Maui.Alerts in order to copy the HEX value by clicking the image next to the HEX value text
