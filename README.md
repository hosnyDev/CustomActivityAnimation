# CustomActivityAnimation

###### in style file
```
    <!-- Base application theme. -->
    <style name="AppTheme" parent="Theme.AppCompat.Light.NoActionBar">
        <!-- Customize your theme here. -->
        <item name="colorPrimary">@color/colorPrimary</item>
        <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
        <item name="colorAccent">@color/colorAccent</item>

        <!-- here call CustomActivityAnimation style  -->
        <item name="android:windowAnimationStyle">@style/CustomActivityAnimation</item>

    </style>

    <!-- Animation when bake or intent -->
    <style name="CustomActivityAnimation" parent="@android:style/Animation.Activity">
        <item name="android:activityOpenEnterAnimation">@anim/slide_in_right</item>
        <item name="android:activityOpenExitAnimation">@anim/slide_out_left</item>

        <item name="android:activityCloseEnterAnimation">@anim/slide_in_left</item>
        <item name="android:activityCloseExitAnimation">@anim/slide_out_right</item>
    </style>

```

## anim folder 

###### slide_in_right file
```
<?xml version="1.0" encoding="utf-8"?>
<set xmlns:android="http://schemas.android.com/apk/res/android">

    <translate
        android:duration="400"
        android:fromXDelta="100%"
        android:fromYDelta="0%"
        android:toXDelta="0%"
        android:toYDelta="0%" />
</set>
```

###### slide_out_left file
```
<?xml version="1.0" encoding="utf-8"?>
<set xmlns:android="http://schemas.android.com/apk/res/android">

    <translate
        android:duration="400"
        android:fromXDelta="0%"
        android:fromYDelta="0%"
        android:toXDelta="-100%"
        android:toYDelta="0%" />
</set>
```

###### slide_in_left file
```
<?xml version="1.0" encoding="utf-8"?>
<set xmlns:android="http://schemas.android.com/apk/res/android">

    <translate
        android:duration="400"
        android:fromXDelta="-100%"
        android:fromYDelta="0%"
        android:toXDelta="0%"
        android:toYDelta="0%" />
</set>
```

###### slide_out_right file
```
<?xml version="1.0" encoding="utf-8"?>
<set xmlns:android="http://schemas.android.com/apk/res/android">

    <translate
        android:duration="400"
        android:fromXDelta="0%"
        android:fromYDelta="0%"
        android:toXDelta="100%"
        android:toYDelta="0%" />
</set>
```
