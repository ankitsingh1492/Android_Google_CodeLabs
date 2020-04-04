# Android Trivia

The starter app was provided by Udacity. It's info can be found [here](https://github.com/udacity/andfun-kotlin-android-trivia/tree/starter-code#how-to-use-this-repo-while-taking-the-course)
This is the app for lesson 3 of the [Android App Development in Kotlin course on Udacity](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012).

## Android Trivia 

The App intends to teach about Fragments and Navigation.


## Learning 1
* A fragment is a part of an activity.
* Created a new Fragment and inflated it with the layout using DatabindingUtil.inflate.
* Should always return the binding root.
* Added Fragment in the Main Activity layout.

## Learning 2
* Added Navigation Component to the build.
* Added Navigation Graph to the build.(Navigation component uses a navigation graph to manage the
app's navigation. The Navigation Graph is a resource file that contains all the app's destinations and
routes)
* Added different fragments to the navigation graph.
* Handled navigation on click of Play button.
* Used Navigation.createNavigateOnClickListener for navigation.

## Learning 3
* Added conditional rendering to the application
* Used view.findNavController().navigate(R.id.action_gameFragment_to_gameOverFragment) for navigation.

## Learning 4
* Did back stack manipulation by setting the pop behavior to popTo inclusive.
* Added more onClick handlers that did some navigation stuff.
```
binding.nextMatchButton.setOnClickListener{view: View ->
              view.findNavController().navigate(R.id.action_gameWonFragment_to_gameFragment)}
```

## Learning 5
* Link the NavController to the ActionBar with NavigationUI.setupWithNavController

## Learning 6
* Created a Menu Resource.
* override onOptionsItemSelected to connect it to our NavigationUI.