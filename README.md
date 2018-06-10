# DiscrollView 2

Updated and revised version of flavienlaurent's [DiscrollView](https://github.com/flavienlaurent/discrollview).

## Compatibilty

API Level 15+

## Download

[![](https://jitpack.io/v/egek92/discrollview2.svg)](https://jitpack.io/#egek92/discrollview2)

### build.gradle(Project)

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
 ### build.gradle(Module:app)
  
  	dependencies {
	        implementation 'com.github.egek92:discrollview2:v1.0'
	}


## Usage

### DiscrollView

```
<!-- Use DiscrollView as your root view in your layout -->

<us.egek.discrollview2.DiscrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:discrollve="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

  <us.egek.discrollview2.DiscrollViewContent
      android:layout_width="match_parent"
      android:layout_height="match_parent">
      
      
      
      
      
      <!-- put your discrollvable views here -->
      
      
      
      
      
        </us.egek.discrollview2.DiscrollViewContent>
</us.egek.discrollview2.DiscrollView>

```

### Discrollvable views

* **alpha**
```
discrollve:discrollve_alpha="true
```
* **scale**
```
discrollve:discrollve_scaleX="true"
discrollve:discrollve_scaleY="true"
```
* **translation**
```
discrollve:discrollve_translation="fromLeft"
discrollve:discrollve_translation="fromRight"
discrollve:discrollve_translation="fromBottom"
discrollve:discrollve_translation="fromTop"
```
you can also combine:
```
discrollve:discrollve_translation="fromRight | fromBottom"
```

* **background color**

from cyan to pink:
```
discrollve:discrollve_fromBgColor="#00b8d4"
discrollve:discrollve_toBgColor="#c51162"
```

## See DiscrollView 2 in action:

![alt tag](https://giant.gfycat.com/FeminineWarlikeEquestrian.gif)

## Sample Code:

```

<?xml version="1.0" encoding="utf-8"?>
<us.egek.discrollview2.DiscrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:discrollve="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

  <us.egek.discrollview2.DiscrollViewContent
      android:layout_width="match_parent"
      android:layout_height="match_parent">

    <TextView
        android:layout_width="match_parent"
        android:layout_height="600dp"
        android:background="@android:color/white"
        android:textColor="@android:color/black"
        android:padding="25dp"
        android:textSize="72sp"
        android:gravity="center"
        android:text="Welcome to DiscrollView 2" />

    <View
        android:layout_width="match_parent"
        android:layout_height="200dp"
        android:background="@color/colorPrimaryDark"
        discrollve:discrollve_alpha="true"
        discrollve:discrollve_threshold="0.3" />

    <ImageView
        android:layout_width="200dp"
        android:layout_height="120dp"
        discrollve:discrollve_alpha="true"
        discrollve:discrollve_translation="fromRight|fromBottom"
        android:src="@android:drawable/ic_dialog_alert" />

    <View
        android:layout_width="match_parent"
        android:layout_height="200dp"
        discrollve:discrollve_fromBgColor="@color/colorPrimary"
        discrollve:discrollve_toBgColor="@color/colorAccent" />

    <ImageView
        android:layout_width="220dp"
        android:layout_height="110dp"
        android:layout_gravity="end"
        android:src="@android:drawable/ic_btn_speak_now"
        discrollve:discrollve_translation="fromRight" />

    <TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:padding="20dp"
        android:gravity="center"
        android:text="Fancy layout"
        android:textSize="18sp"
        discrollve:discrollve_alpha="true"
        discrollve:discrollve_translation="fromTop" />

    <ImageView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="20dp"
        android:layout_gravity="center"
        android:src="@android:drawable/ic_delete"
        discrollve:discrollve_scaleX="true"
        discrollve:discrollve_scaleY="true"  />

  </us.egek.discrollview2.DiscrollViewContent>
</us.egek.discrollview2.DiscrollView>

```
