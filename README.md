Fragments

A fragment is an independent Android component which can be used by an activity. A fragment encapsulates functionality so that it is easier to reuse within activities and layouts. A fragment runs in the context of an activity, but has its own life cycle and typically its own user interface.Sep 22, 2020

Why fragments are used in Android?

Passing information between app screens

Historically each screen in an Android app was implemented as a separate Activity. ... By making each screen a separate Fragment, this data passing headache is completely avoided. Fragments always exist within the context of a given Activity and can always access that Activity

Difference between fragment and activity

Fragment	Activity
Fragment represents a behavior or a portion of user interface in an Activity.	Activity is the part where the user will interacts with your application.
A fragment can be reused in multiple activities, so it acts like a reusable component in activities. 	The activity has own life cycle but fragment has there own life cycle. For Activity, we just need to mention in Manifest but for fragment its not required.

Fragment represents a behavior or a portion of user interface in an Activity. You can combine multiple fragments in a single activity to build a multi-pane UI and reuse a fragment in multiple activities


What is the Back Stack?

A task is a collection of activities that users interact with when performing a certain job. The activities are arranged in a stack—the back stack) in the order in which each activity is opened. 

If the user presses the Back button, that new activity is finished and popped off the stack.

Fragment Back Stack Managment

FragmentManager is the class responsible for performing actions on your app's fragments, such as adding, removing, or replacing them, and adding them to the back stack.


Principles of Navigation

First Principle
* There’s always a starting place

Second Principle
* You can always go back 
* It is also known as back stack

Third Principle
* Up goes back (mostly)


Action	Definition
PopTo Non-Inclusive	Pops off everything on the back stack until it finds the referenced fragment transactions.
PopTo Inclusive	Pops offs everything on the back stack, including the referenced fragment transaction.


￼


What is Android Bundle ?

Android Bundle is used to pass data between activities. The values that are to be passed are mapped to String keys which are later used in the next activity to retrieve the values. Following are the major types that are passed/retrieved to/from a Bundle.


What is intent and intents filter?

An Intent is a messaging object you can use to request an action from another app component. Although intents facilitate communication between components in several ways, there are three fundamental use cases:


* Explicit intents

specify which application will satisfy the intent, by supplying either the target app's package name or a fully-qualified component class name. You'll typically use an explicit intent to start a component in your own app, because you know the class name of the activity or service you want to start. For example, you might start a new activity within your app in response to a user action, or start a service to download a file in the background.

Launch specific activity

* Implicit intents 
do not name a specific component, but instead declare a general action to perform, which allows a component from another app to handle it. For example, if you want to show the user a location on a map, you can use an implicit intent to request that another capable app show a specified location on a map.

Specify what you want done and system chooses activity


Intent Action

The type of thing that the app wants to have done on its behalf.

Common Action

Action_view
Action_dial
Action_edit

Intent Category

Adds a subtype to the action

* Category_App_Music
* Category_App_Email
* Category_App_Maps
* Category_App_Gallery
* Category_App_Calculator
* Category_App_Calendar


Intent Data Type

MIME Data Type
Allow activities to support specific data types.

￼
