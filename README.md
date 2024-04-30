# nav-plugin
nav-plugin Plugin
This is a Gradle plugin used to collect all Activity and Fragment pages in a project, used in conjunction with the Jetpack Navigation framework.

Example:

Step 1: 
```kotlin
@NavDestination(type=NavType.Fragment, route="home_fragment") 
class HomeFragment: Fragment {

}

@NavDestination(type=NavType.Activity, route="home_activity") 
class HomeActivity: FragmentActivity {

}
```

Step 2: 
```kotlin
class MainActivity : FragmentActivity {
    fun onCreate(bundle: Bundle) {
        NavRegistry.DESTINATIONS
    }
}
```
