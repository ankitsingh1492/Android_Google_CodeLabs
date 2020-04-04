# Activity Lifecycle - DessertPusher

# DessertPusher

The starter app was provided by Udacity. It's info can be found [here](https://github.com/udacity/andfun-kotlin-dessert-pusher/tree/starter-code#how-to-use-this-repo-while-taking-the-course)
This is the app for lesson 4 of the [Android App Development in Kotlin course on Udacity](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012).
The lesson is about Activity lifecycle.

## Learning 1
* Added the logs.
* Added Timber to the project.
* Created Application Class - An Application class in android is the base class inside android application that
 contains all the other components. The Application class, or any subclass of the Application class, is instantiated
 before any other class when the process for your application/package is created. This class is only used for
 initialization of global state before the first Activity is displayed.

 ### Lifecycle States - (Udacity Notes)

 [Lifecycle Summary](https://youtu.be/efYCAKJBq5k)

 Following are the lifecycle states which are same for both Activity and Fragment.

 * Initialized - Starting state of a new activity. It directly goes to Created.
 * Created - Activity created but not yet visible and focused .
 * Started - Activity visible but not focused.
 * Resumed - Activity is running, both visible and focused.
 * Destroyed - Activity is removed from memory or destroyed.


### Activity Lifecycle Callbacks - (Udacity Notes)

* onCreate() -  Called the first time the activity starts and is only called once during the lifecycle of the activity.
* onStart() - Triggered when the activity is about to become visible.
* onResume() - Triggered when activity is focused.
* onPause() - Triggered when activity just loses focus.
* onStop() - mirror method of onStart(). When the user cannot see the activity.
* onDestroy() - mirror method of onCreate()

[Useful Link 1](https://medium.com/androiddevelopers/the-android-lifecycle-cheat-sheet-part-i-single-activities-e49fd3d202ab)
