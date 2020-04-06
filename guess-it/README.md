# Application Architecture

The starter app was provided by Udacity. It's info can be found [here](https://github.com/udacity/andfun-kotlin-guess-it/tree/starter-code#how-to-use-this-repo-while-taking-the-course)
This is the app for lesson 5 of the [Android App Development in Kotlin course on Udacity](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012).


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
* Is lifecycle aware.

THe observer pattern is where we have objects called a subject. THe subject keeps track of other objects known as observers.
The observers watch subject when the status of subject changes it notifies the observers by calling a method in the observers.
In livedata case the subject is livedata object and the observers are the UIControllers.

LINKS
* [Talk - Fun with livedata](https://www.youtube.com/watch?v=2rO4r-JOQtA)
* [Documentation - Handling Lifecycles](https://developer.android.com/topic/libraries/architecture/lifecycle)
* [Documentation - LiveData](https://developer.android.com/topic/libraries/architecture/livedata)

* Added LiveData encapsulation to the GameViewModel
* Using Kotlin Property called [backing Property](https://kotlinlang.org/docs/reference/properties.html#backing-properties)
* [Kotlin automatically makes getters and setters for our fields](https://kotlinlang.org/docs/reference/properties.html#getters-and-setters)

# Learning 3

## View Model Factory

A class that knows how to create [ViewModels](https://developer.android.com/reference/kotlin/androidx/lifecycle/ViewModelProvider.Factory.html)

## Adding a Constructor

* Create a ViewModel that takes in a constructor parameter.
* Make a ViewModel Factory for ViewModel
* Have factory construct ViewModel with constructor parameter.
* Add ViewModel Factory when using ViewModelProviders.
* Need when we need a value right when a viewmodel is initialized.

# Learning 4

* Data binding.

ViewModel can communicate directly to the view. without UI Controller being in the middle,

LINKS
* [Documentation-Layouts and binding expressions](https://developer.android.com/topic/libraries/data-binding/expressions)
* [Documentation- Listener Bindings](https://classroom.udacity.com/courses/ud9012/lessons/da3967cc-ba85-4045-bb46-dea1c770fb8b/concepts/(https://developer.android.com/topic/libraries/data-binding/expressions#listener_bindings)
* [Documentation - Use ViewModel to Manage UI-related data](https://developer.android.com/topic/libraries/data-binding/architecture#viewmodel)
