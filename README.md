## FabAnimator 
[![](https://jitpack.io/v/okabbas/FabAnimator.svg)](https://jitpack.io/#okabbas/FabAnimator)
[![License](http://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://github.com/okabbas/FabAnimator)

This library is for adding smooth animation and animators to the FloatingActionButton library android.


<img src="assets/sample.gif">


## Getting Started :
Add to your root build.gradle :
```Groovy
allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
    }
  }
```

Add the dependency :
```Groovy
dependencies {
    implementation 'com.github.okabbas:FabAnimator:0.9.2'
}
```

## Simple API :

##### In `Kotlin`:
```Groovy
val animatorObject = AnimatorObject(fab_1)

animatorObject.createAnimator() //To start animations by default

animatorObject.stopAnimator() //To stop animations by default

//So easy :) I love Kotlin :)
```

##### In `Java` :
```Groovy
  AnimatorObject animatorObject = new AnimatorObject(fab_1);
  
  AnimatorObject.createAnimator(ColorModel.Background,
  AnimModel.None, 300, new int[]{Color.MAGENTA, Color.RED}); //To start animations by default

  AnimatorObject.stopAnimator(ColorModel.Background, Color.BLACK); //To stop animations by default
```

## Advanced API :

##### In `Kotlin`:
###### [Sample code written with Katlin](Sample/src/main/kotlin/com/github/okabbas/FabAnimator.Sample/kotlin.kt).

##### In `Java`:
###### [Sample code written with Java](Sample/src/main/kotlin/com/github/okabbas/FabAnimator.Sample/java.kt).

## License
    MIT License

    Copyright (c) 2018 Abbas Naghdi

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
