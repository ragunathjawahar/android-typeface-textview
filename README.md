Typeface TextView
----------------

Typeface TextView allows you to specify custom fonts right in the XML and avoids typeface 
creation boilerplate code.

Quick Start
-----------
**Step 1 - Add Typeface TextView as a library project**

**Step 2 - Make the highlighted changes to your XML layout**
```xml
<!-- 1. Add a custom namespace, xmlns:geekui -->
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:geekui="http://schemas.android.com/apk/res-auto"
    android:layout_width="fill_parent"
    android:layout_height="fill_parent">

    <!-- 2. Replace <TextView> tags with <com.mobsandgeeks.ui.TypefaceTextView> tags -->
    <!-- 3. Specify the path to your custom font in the 'assets' folder
            using the 'geekui:customTypeface' attribute -->
    <com.mobsandgeeks.ui.TypefaceTextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/hello_world"
        geekui:customTypeface="fonts/custom_font.ttf" />

</RelativeLayout>
```

License
-------

    Copyright 2013 Mobs and Geeks

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
