# Workshop1
First Android Workshop

## TODO

### Remove ToolBar
Add in **styles.xml**:
```xml
<style name="AppTheme.NoActionBar">
        <item name="windowActionBar">false</item>
        <item name="windowNoTitle">true</item>
</style>
```

Change in `AndroidManifest.xml` so it look like this:
```java
<activity android:name=".MainActivity"
            android:theme="@style/AppTheme.NoActionBar">
```

### Set Background
Add in **colors.xml"":
```java
    <color name="bgStart">#5D2469</color>
    <color name="bgEnd">#672DD1</color>
```

Add in **drawable** folder file **background.xml**
```java
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android">
    <gradient
        android:angle="45"
        android:startColor="@color/bgStart"
        android:endColor="@color/bgEnd"
        />
</shape>
```

Add in **activity_main.xml**:
````java
android:background="@drawable/background"
```