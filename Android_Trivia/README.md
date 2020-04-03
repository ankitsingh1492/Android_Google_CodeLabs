# Android Trivia

The starter app was provided by Udacity. It's info can be found [here](https://github.com/udacity/andfun-kotlin-android-trivia/tree/starter-code#how-to-use-this-repo-while-taking-the-course)
This is the app for lesson 3 of the [Android App Development in Kotlin course on Udacity](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012).

## Android Trivia 


The Android Trivia application is an application that asks the user trivia questions about Android development.  It makes use of the Navigation component within Jetpack to move the user between different screens.  Each screen is implemented as a Fragment.
The app navigates using buttons, the Action Bar, and the Navigation Drawer.


## Learning 1
* A fragment is a part of an activity.
* Created a new Fragment and inflated it with the layout using DatabindingUtil.inflate.
* Should always return the binding root.
* Added Fragment in the Main Activity layout.


#Learning 2
* Added Navigation Component to the build.
* Added Navigation Graph to the build.(Navigation component uses a navigation graph to manage the
app's navigation. The Navigation Graph is a resource file that contains all the app's destinations and
routes)
* Added different fragments to the navigation graph.
* Handled navigation on click of Play button.
* Used Navigation.createNavigateOnClickListener for navigation.