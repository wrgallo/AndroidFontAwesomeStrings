# AndroidFontAwesomeStrings
String resources for the free FontAwesome icons for use with AndroidStudio.

1. First create your **Font Resource Directory**
   1. Right-click the **res** folder and go to **New > Android resource directory**
   1. In the *Resource type list*, select *font*, and then click **OK**
   1. Check [this guide](https://developer.android.com/guide/topics/ui/look-and-feel/fonts-in-xml) for more details
1. Download the FontAwesome TTF files
   * Brands Icons: **[fa-brands-400.ttf](https://github.com/FortAwesome/Font-Awesome/blob/master/webfonts/fa-brands-400.ttf)**
   * Regular Icons: **[fa-regular-400.ttf](https://github.com/FortAwesome/Font-Awesome/blob/master/webfonts/fa-regular-400.ttf)**
   * Solid Icons **[fa-brands-900.ttf](https://github.com/FortAwesome/Font-Awesome/blob/master/webfonts/fa-solid-900.ttf)**
1. Add your font files in the **font** folder
   1. Right-click the **font** folder and go to **Show in Explorer**
   2. Move your desired TTF files to this folder
1. Create your icon dictionary:
   1. Right-click the **values** resources folder and go to **Show in Explorer**
   1. Move the [XML Files](https://github.com/wrgallo/AndroidFontAwesomeStrings) to this folder:
       * XML for Brands Icons: `strings_fa_brands.xml`
       * XML for Regular Icons: `strings_fa_regular.xml`
       * XML for Solid Icons: `strings_fa_solid.xml`
   1. Or check the [FontAwesome Cheatsheet](https://fontawesome.com/cheatsheet) to create your own, the XML will look like this:

    ```XML
    <resources>
       <string name="fa_regular_sun">&#xf185;</string>
  	   <string name="fa_regular_surprise">&#xf5c2;</string>
	   <string name="fa_regular_thumbs_up">&#xf164;</string>
   </resources>
    ```
1. In the layout XML file, set the `text` and `fontFamily` attribute to the icon you want
    ```XML
    <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/fa_regular_thumbs_up"
            android:fontFamily="@font/fa-regular-400"/>
    ```
