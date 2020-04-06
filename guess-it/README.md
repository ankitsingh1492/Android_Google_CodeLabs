# Application Architecture

The starter app was provided by Udacity. It's info can be found [here](https://github.com/udacity/andfun-kotlin-guess-it/tree/starter-code#how-to-use-this-repo-while-taking-the-course)
This is the app for lesson 4 of the [Android App Development in Kotlin course on Udacity](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012).


# Learning 1

## Architecture

LINKS

* [Code samples - Android Architecture blueprints](https://github.com/android/architecture-samples)
* [Talk , Google I/O](https://www.youtube.com/watch?v=pErTyQpA390)
* [Talk - Droidcon NYC 2016 - A Journey Through MV Wonderland](https://www.youtube.com/watch?v=QrbhPcbZv0I)
* [Blog Post - Android Architecture Patterns Part 2: Model-View-Presenter](https://medium.com/upday-devs/android-architecture-patterns-part-2-model-view-presenter-8a6faaae14a5)
* [Documentation - Guide to App Architecture](https://developer.android.com/jetpack/docs/guide)
* [Blog Post - Android and architecture](https://android-developers.googleblog.com/2017/05/android-and-architecture.html)

## View Model -
Abstract class that holds the app's UI data.

LINKS

* [Documentation](https://developer.android.com/topic/libraries/architecture/viewmodel)
* [View Models : A simple example](https://medium.com/androiddevelopers/viewmodels-a-simple-example-ed5ac416317e)

## Adding a View Model

* Add dependency.
* Subclass ViewModel.
* Associated UI controller and ViewModel.

## ViewModel vs UI Controller

* ViewModel holds data for UI.
* UI Controller only displays and gets user/OS events.
* UI Controller does not make decisions.
* ViewModel never references fragments, activities and views.

LINKS
* [Saving States](https://developer.android.com/topic/libraries/architecture/saving-states)
* [Blog - ViewModels: Persistence, onSaveInstanceState](https://medium.com/androiddevelopers/viewmodels-persistence-onsaveinstancestate-restoring-ui-state-and-loaders-fc7cc4a6c090)

# Learning 2

## Live Data
Live data is an observable data holder class that is lifecycle-aware.

* Live data wraps arounds a data.
* Live data is observable.

THe observer pattern is where we have objects called a subject. THe subject keeps track of other objects known as observers.
The observers watch subject when the status of subject changes it notifies the observers by calling a method in the observers.
In livedata case the subject is livedata object and the observers are the UIControllers.