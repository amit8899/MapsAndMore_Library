# MapsAndMore_Library
###Android Library

> Step 1. Add the JitPack repository to your build file

```gradle
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  ```
  
> Step 2. Add the dependency
  
  ```gradle
  dependencies {
	        implementation 'com.github.amit8899:MapsAndMore_Library:Tag'
	}
 ```
 
 > Step 3. Initialise MapsAndMore as object 
 *Pass your Main activity*
 *linear layout where you want the popup message*
 ```MapsAnfMore object = new MapsAndMore(activity, applogo, linearlayout);
 ```
 
 > Step 4. Add this in your button onclickListener
 ```
    object.start();
    // for starting or stopping service
 ```
 
 > Step 5. Get location permission 
 *This method takes true or false depends on the location permission*
 ```
    object.passPermission(permission);
 ```
 
 > Step 6. Add this in OnResume of your activity
 ```
    object.configure();
 ```
 
 
