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
	        compile 'com.github.egek92:discrollview2:v1.0'
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

