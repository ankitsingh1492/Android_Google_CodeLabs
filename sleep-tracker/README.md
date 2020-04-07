# SleepQualityTracker

The starter app was provided by Udacity. It's info can be found [here](https://github.com/udacity/andfun-kotlin-sleep-tracker)
This is the app for lesson 6 of the [Android App Development in Kotlin course on Udacity](https://www.udacity.com/course/developing-android-apps-with-kotlin--ud9012).

This app demonstrates the following views and techniques:
* Room database
* DAO
* Coroutines

It also uses and builds on the following techniques from previous lessons:
* Transformation map
* Data Binding in XML files
* ViewModel Factory
* Using Backing Properties to protect MutableLiveData
* Observable state LiveData variables to trigger navigation


# Learning 1 - 

* Entity - Object or concept to store in the database. Entity class defines a table. Each instance is stored as a table row.
* [Defining data using Room entities](https://developer.android.com/training/data-storage/room/defining-data.html)
* [ColumnInfo](https://developer.android.com/reference/android/arch/persistence/room/ColumnInfo)
* [List of all Room Annotations](https://developer.android.com/reference/android/arch/persistence/room/package-summary#annotations)

# Learning 2 -

### DAO

Defining and calling kotlin functions in your code that map to sql queries.
You define those mappings in a DAO or Database Access Obj using annotations and room creates the necessary code for you.
Think of DAO as defining a custom interface for accessing your DB.

DAO annotations
@insert , @delete, @update, @query

LINKS

* [DAO](https://developer.android.com/reference/android/arch/persistence/room/Dao.html)
* [Room Persistence Library](https://developer.android.com/training/data-storage/room/index.html)

# Learning 3 -

### Creating a Room DB

* Create a Public Abstract class that extends roomDataBase.
* Annotate the class as DataBase.
* Associate with DAO.
* Get once instance/reference of DataBase.

## Developer Documentations-

* [Room Database](https://developer.android.com/reference/android/arch/persistence/room/RoomDatabase)
* [Database  - Annotations](https://developer.android.com/reference/android/arch/persistence/room/Database)
* [Raw Queries with Room](https://developer.android.com/reference/android/arch/persistence/room/RawQuery)
* [On Properly using volatile and synchronized](https://developer.android.com/jetpack/docs/guide#separation-of-concerns)
* [Companion Objects](Companion objects)
* [Understanding Migrations with ROOM](https://medium.com/androiddevelopers/understanding-migrations-with-room-f01e04b07929)
