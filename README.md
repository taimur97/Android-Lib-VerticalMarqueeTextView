Vertical Marquee TextView for Android
=====================================

[ ![Download](https://api.bintray.com/packages/ayltai/maven/Android-Lib-VerticalMarqueeTextView/images/download.svg) ](https://bintray.com/ayltai/maven/Android-Lib-VerticalMarqueeTextView/_latestVersion)

A custom TextView with vertical marquee effect.

<img src="https://raw.github.com/ayltai/Android-Lib-VerticalMarqueeTextView/master/screenshots/device-2014-02-22-000150.png" width="240" height="400" alt="Screenshot-1" />&nbsp;
<img src="https://raw.github.com/ayltai/Android-Lib-VerticalMarqueeTextView/master/screenshots/device-2014-02-22-000158.png" width="240" height="400" alt="Screenshot-2" />&nbsp;
<img src="https://raw.github.com/ayltai/Android-Lib-VerticalMarqueeTextView/master/screenshots/device-2014-02-22-000208.png" width="240" height="400" alt="Screenshot-3" />

Features
--------

* Automatically start marquee effect when the TextView is added to a view.
* Customizable marquee speed
* Easy to extend and customize

Installation
------------

<pre>
repositories {
    jcenter()
}

dependencies {
    compile 'android.lib.verticalmarqueetextview:VerticalMarqueeTextView:+'
}
</pre>

How to use
----------

This project includes an [activity_example.xml](https://github.com/ayltai/Android-Lib-VerticalMarqueeTextView/blob/master/Samples/src/main/res/layout/activity_example.xml) to show how to use this library using XML declaration. An [ExampleActivity](https://github.com/ayltai/Android-Lib-VerticalMarqueeTextView/blob/master/Samples/src/main/java/android/lib/widget/verticalmarqueetextview/ExampleActivity.java) is also included, which, however, is basically empty because you don't need to write any code!

Here is the example layout that generates the above screenshots:

    <?xml version="1.0" encoding="utf-8"?>
    <LinearLayout
        xmlns:android="http://schemas.android.com/apk/res/android"
        xmlns:example="http://schemas.android.com/apk/res-auto"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical">
        <ImageView
            android:layout_width="wrap_content"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:layout_gravity="center_horizontal"
            android:scaleType="centerInside"
            android:src="@android:drawable/sym_def_app_icon" />
        <android.lib.verticalmarqueetextview.VerticalMarqueeTextView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:layout_gravity="center_horizontal"
            example:marqueeSpeed="25"
            example:textSize="20dp"
            example:textColor="@android:color/white"
            example:textStyle="bold"
            example:text="The quick brown fox jumps over the lazy dog. The quick brown fox jumps over the lazy dog. The quick brown fox jumps over the lazy dog. The quick brown fox jumps over the lazy dog." />
        <View
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1" />
    </LinearLayout>