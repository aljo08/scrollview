ScrollingText (Android)

A simple Android app written in Java that displays a longer article in a scrolling view with a two-column layout: a narrow left column for the subtitle and a wide right column for the article text. Created as an assignment for the course Razvoj mobilnih aplikacij (Mobile Application Development), Task 4.

Features
Article title shown in a blue header
Narrow left column (100dp) with the subtitle
Wide right column with the article text (layout_width="0dp" + layout_weight="1")
Whole content is placed inside a ScrollView, so the long text can be scrolled vertically
Bold and italic parts of the text defined directly in strings.xml
Web address in the article is clickable (autoLink="web")
Add comment button at the bottom that shows a Toast with the message Comment submitted!
All texts are stored in strings.xml, none are hardcoded in the layout
Project structure
app/src/main/
├── java/com/example/scrollview/MainActivity.java   # Toast on button click
└── res/
    ├── layout/activity_main.xml                    # ScrollView layout
    └── values/strings.xml                          # title, subtitle, article, button text
How it works
ScrollView contains exactly one direct child: a vertical LinearLayout.
Inside it are the title TextView, a horizontal LinearLayout with the two columns (subtitle and article) and the button.
The button uses android:onClick="showComment". The method showComment(View view) in MainActivity is public void and displays the Toast.
Requirements
Android Studio (recent version)
Android SDK, minimum API level as set in the project
Android emulator or a physical Android phone
Running the app
Clone the repository:
   git clone https://github.com/aljo08/Scrollview.git
Open the project in Android Studio (File → Open).
Wait for the Gradle sync to finish.
Select a device and click Run.
Running on a physical phone
Enable Developer options (tap Build number 7 times in Settings → About phone).
Turn on USB debugging (or Wireless debugging on Android 11+).
Connect the phone, confirm the debugging prompt and select it in the device drop-down in Android Studio.
Screenshots

Add screenshots to a screenshots/ folder and link them here:


Author

GitHub: aljo08

Student project – Mobile Application Development, Task 4.
