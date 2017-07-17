# PagingKit
PagingKit provides customisable menu & content UI.

![Swift 3.0+](https://img.shields.io/badge/Swift-3.0+-orange.svg)
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)

![paging_sample](https://user-images.githubusercontent.com/18320004/27948466-d94665b8-6334-11e7-8bd8-a5d28eddb797.gif)


# What's this?
There are many libaries providing "Paging UI" which has menu and content area.
They are convinience but not customizable because your app have to make compatible with the library about layout and design.
When It doesn't fit the libaries, you need to fork the library or find another one. 

PagingKit has more flexible layout and design than the other libraries.
You can construct "Menu" and "Content" UI, and they work together. That's all features this library provides.
You can fit layout and design of Pagingin UI to your apps as you like.

For example:

| changing position of Menu and Content | placing a view between Menu and Content |
|:------------:|:------------:|
| ![paging_sample3](https://user-images.githubusercontent.com/18320004/27946963-fc4d0ee6-632e-11e7-9bcb-1cf171ffdc88.gif) | ![paging_sample2](https://user-images.githubusercontent.com/18320004/27946966-fe94c216-632e-11e7-96db-d8e0ec9acecb.gif) |


| tag like menu desing | text highlighted menu design |
|:------------:|:------------:|
| ![tag](https://user-images.githubusercontent.com/18320004/28256285-bbf663b8-6afb-11e7-9779-7d9716dbb87a.gif) | ![overlay](https://user-images.githubusercontent.com/18320004/28256286-bd274f40-6afb-11e7-8662-7fea65b608f3.gif) |



# Feature
- [x] easy to costruct Paging UI many media Apps have
- [x] customizable layout and design
- [x] UIKit like API

# Requirements
+ iOS 8.0+
+ Xcode 8.1+
+ Swift 3.0+

# Installation
## Carthage
+ Install Carthage from Homebrew
```
> ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
> brew update
> brew install carthage
```
+ Move your project dir and create Cartfile
```
> touch Cartfile
```
+ add the following line to Cartfile
```
github "kazuhiro4949/PagingKit"
```
+ Create framework
```
> carthage update --platform iOS
```

+ In Xcode, move to "Genera > Build Phase > Linked Frameworks and Library"
+ Add the framework to your project
+ Add a new run script and put the following code
```
/usr/local/bin/carthage copy-frameworks
```
+ Click "+" at Input file and Add the framework path
```
$(SRCROOT)/Carthage/Build/iOS/PagingKit.framework
```
+ Write Import statement on your source file
```
Import PagingKit
```

# Usage


# Class Design
# License

Copyright (c) 2017 Kazuhiro Hayashi

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
