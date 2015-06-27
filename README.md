# 360-Productview-Android-App
This is a 360 degree product view seeing in shoppingcart sites.like view selcted product by roatating for android, build with jquery runs prefectly in webview.


#1)jQuery Plugin For Draggable 360 Degrees Product Image View - j360 ([Link](http://www.jqueryscript.net/rotator/jQuery-Plugin-For-Draggable-360-Degrees-Product-Image-View-j360.html)) 
an MIT Licence

#2)jquery.min.js ([Link](http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js)) 

## VIDEO ([SAMPLE](https://www.youtube.com/watch?v=YsNO7LKqJcs))   
   
Some Screenshots are given below
<p><b>On Rotation</b></p>
<p><a href="https://github.com/rameshvoltella/360-Productview-Android-App/blob/master/Screenshot_2015-06-27-22-32-03.png" target="_blank"><img src="https://github.com/rameshvoltella/360-Productview-Android-App/blob/master/Screenshot_2015-06-27-22-32-03.png" alt="On Rotation" style="max-width:100%;"></a></p>

<p><b>On Rotation :)</b></p>
<p><a href="https://github.com/rameshvoltella/360-Productview-Android-App/blob/master/Screenshot_2015-06-27-22-32-07.png" target="_blank"><img src="https://github.com/rameshvoltella/360-Productview-Android-App/blob/master/Screenshot_2015-06-27-22-32-07.png" alt="On Rotation" style="max-width:100%;"></a></p>


<p><b>On Rotation :)</b></p>
<p><a href="https://github.com/rameshvoltella/360-Productview-Android-App/blob/master/Screenshot_2015-06-27-22-32-12.png" target="_blank"><img src="https://github.com/rameshvoltella/360-Productview-Android-App/blob/master/Screenshot_2015-06-27-22-32-12.png" alt="On Rotation :)" style="max-width:100%;"></a></p>


Hash-Tags: how to use
------------------------


1. Use the Custum WebView ProductShowCaseWebView

```xml
<yourpackagename.ProductShowCaseWebView
        android:id="@+id/web_view"
        android:layout_width="fill_parent"
        android:layout_height="fill_parent" />
```
2 Cast in java

```java
       ProductShowCaseWebView wv = (ProductShowCaseWebView) findViewById(R.id.web_view);
```
3 Add images you need to use for the 360 view

```java
       String imagesTag360="";

        /*Taking images from the assert folder*/

        for(int i=1;i<19;i++)
        {
            imagesTag360=imagesTag360+"<img src=\"file:///android_asset/images/image1_"+i+".jpg\"/>" ;
        }
```
4 To use images from url for 360 view
```java
String imagesTag360="";

        /*Taking images from urlr*/
        int imageCount=19//Just for a example u can use any number, like size of imagelist(While you parse set of images to shown in the view)

        for(int i=1;i<imageCount;i++)
        {
            imagesTag360=imagesTag360+"<img src=\"http://imageurl.com/image1_.jpg\"/>" ;
        }
```        
        
5  To make 360 degree draggable View

```java
  wv.loadDataWithBaseURL("",
                imagesTag360, "text/html", "UTF-8", null);
 ```               






## License

    The MIT License (MIT)

    Copyright (c) 2015 Ramesh M Nair
 
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

     THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.





