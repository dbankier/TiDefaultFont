# TiDefaultFont

Set the __default__ _custom_ font in your Titanium Android application. Affects all native elements, e.g. action bars, tabs, dialogs as well as
acts as the default font for all `Ti.UI` elements.

## How To

 * Copy your custom font to: `Resources/fonts` directory

 * Install the module as normal, e.g. with [gitto](http://gitt.io/):

```
$ gittio install yy.defaultfont
```

 * Add the following to your `tiapp.xml`

```
  <property name="ti.android.defaultfont" type="string">fonts/MyFont.ttf</property>
```

 * Add the following to your custom theme:

```
   <item name="android:typeface">serif</item>
```

### Custom Theme Example
In `tiapp.xml`:

```
  <android>
    <manifest>
      <application android:theme="@style/Theme.YY">
      </application>
    </manifest>
  </android>
```

In `platform/android/res/values/style.xml`, e.g.:

```
<resources xmlns:android="http://schemas.android.com/apk/res/android">  
   <style name="Theme.YY" parent="Theme.AppCompat">
        <item name="android:typeface">serif</item>
   </style>         
</resources>
```

### Credits
Mostly based on this: https://gist.github.com/artem-zinnatullin/7749076

### License: MIT
