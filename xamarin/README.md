# Xamarin 

[![N|Solid](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f2/Xamarin-logo.svg/1200px-Xamarin-logo.svg.png)]()

## Table of Contents
1. [Introduction](#introduction)
1. [Installation Guide](#installation-guide)
1. [Xamarin Projects](#xamarin-projects)
1. [Introduction to C#](#introduction-to-c#)
1. [XAML Basics](#xaml-basics)
1. [Data Binding and MVVM](#data-binding-and-mvvm)
1. [Nuget Package Manager](#nuget-package-manager)
1. [Xamarin Forms Controls](#xamarin-forms-controls)
1. [Using Custom Renderers](#using-custom-renderers)
1. [Writing Dependency Services](#writing-dependency-services)

## Introduction
Build native apps for multiple platforms on a shared C# codebase. Use the same IDE, language, and APIs everywhere.
-  Native UI, native API access, and native performance
-  Anything you can do in Objective-C, Swift, or Java you can do in C# with Xamarin
-  Ship cutting-edge apps with same-day support for new OS releases

## Installation Guide
Overview of installation and setup practices that apply across platforms.
-  **[Windows][xamarinWin]** users 
-  Mac users can use **[Xamarin Studio][xamarinStudioMac]** or can download and setup **[Visual Studio][xamarinVisualStudioMac]** for mac

Some pointers as you're performing installation:
-  Now that Visual Studio for Mac is officially released, seems the direction is to move to VS and leave XS behind. After installing VS for Mac.
-  Xamarin Studio will stop receiving updates in coming days to months hence everybody should move to Visual Studio for Mac.

## Xamarin Projects
When developing in Xamarin, you have two options to choose from: Xamarin.Platform and Xamarin.Forms.

[![N|solid](https://image.slidesharecdn.com/developinganddesigningnativemobileappsinvisualstudio-140612112104-phpapp01/95/developing-and-designing-native-mobile-apps-in-visual-studio-13-638.jpg?cb=1403543314)]()

#### Xamarin.Forms
In Xamarin Forms development, more than 90% code is shared across platforms since both the UI and business logic is shared. Dependency services and Renderers can be used to write platform specific code to access functionality not available in Forms.

Xamarin.Forms is best for:
- Apps that require little platform-specific functionality
- Apps where code sharing is more important than custom UI
- Developers comfortable with XAML

#### Xamarin.iOS & Xamarin.Android
Also called Xamarin Native development, is a xamarin project in which the business logic is shared while the UI's are seperate for each platform. This allows for greater control over the App's user experience.

Xamarin.iOS & Xamarin.Android are best for:
- Apps with interactions that require native behavior
- Apps that use many platform-specific APIs
- Apps where custom UI is more important than code sharing

## Introduction to C#
C# is used for Xamarin development. To understand the syntax of C# and find out the data types and structures available, please go through the following [link](https://www.tutorialspoint.com/csharp/csharp_basic_syntax.htm).

- I/O operations, Webservice calls and CPU intensive operations are done in a seperate thread so as not to block the UI Thread; you need to familiarze yourself with [Async and Await](https://docs.microsoft.com/en-us/dotnet/csharp/async).
- [Linq](https://realm.io/docs/xamarin/latest/api/linqsupport.html) comes in handy for performing Data Manipulation on large Lists and Collections.
- [Coding standards](http://www.dofactory.com/reference/csharp-coding-standards) for C#

## XAML Basics
XAML is a markup language and is the prefered way of creating UI in Xamarin Forms. Although, UI can also be created programmatically in code but using XAML provides seperation of concern making the code more manageable.

You can follow [this tutorial](https://developer.xamarin.com/guides/xamarin-forms/xaml/xaml-basics/getting_started_with_xaml/) which gives step-by-step instructions on how to create a simple User Interface in XAML.
*(Tip: Press Ctrl+Space on an added XAML element to view all possible properties you can play with. Intellisense saves lives.)*

If you want more information on XAML, read through this section for more detailed information on XAML.

## Data Binding and MVVM
MVVM architectural pattern is used in Xamarin Forms.

[![N|solid](https://developer.xamarin.com/guides/xamarin-forms/creating-mobile-apps-xamarin-forms/summaries/Images/ch18fg03.png)]()

Use [this turtorial](https://developer.xamarin.com/guides/xamarin-forms/xaml/xaml-basics/data_bindings_to_mvvm/) get hands-on with the MVVM pattern.

## Nuget Package Manager
NuGet is a package management system for .NET that simplifies the process of using third party libraries in your application. 

To find out how to add nuget packages to your projects, [click here](https://blog.xamarin.com/xamarin-studio-and-nuget/).

## Xamarin Forms Controls
Xamarin uses four main control groups to construct the User Interface:
1. [Pages](https://developer.xamarin.com/guides/xamarin-forms/user-interface/controls/pages)
1. [Layouts](https://developer.xamarin.com/guides/xamarin-forms/user-interface/controls/layouts)
1. [Views](https://developer.xamarin.com/guides/xamarin-forms/user-interface/controls/views)
1. [Cells](https://developer.xamarin.com/guides/xamarin-forms/user-interface/controls/cells) 

## Using Custom Renderers
In Xamarin Forms each control is mapped to the corresponding native control of that platform. For e.g; an Entry in Xamarin Forms when rendered on iOS will be a UITextField and on Android will be EditText. 

Custom Renderers can be used to modify the native controls for styling or behavioral changes that are not supported at the Forms level. 

[Follow this](https://developer.xamarin.com/guides/xamarin-forms/application-fundamentals/custom-renderer/entry/) tutorial of an EntryRender, to get a feel of how to write a custom renderer. Detailed information about Renderers can be found [here](https://developer.xamarin.com/guides/xamarin-forms/application-fundamentals/custom-renderer/).

## Writing Dependency Services
Dependency services can be used to access platform specific functionality that is unavailable at the Forms level. 

An interface is created at the Forms level and implemented in each of the native projects. The methods of the interface are used to call the native functionality in Forms where ever required.
*(Tip: Before venturing to write you own Dependency Service, check if it's already available as a NugetPackage. [This](https://github.com/jamesmontemagno/Xamarin.Plugins) is a good place to start.)*

[![N|solid](https://developer.xamarin.com/guides/xamarin-forms/application-fundamentals/dependency-service/introduction/Images/overview_diagram.png)]()

[This tutorial](https://developer.xamarin.com/guides/xamarin-forms/application-fundamentals/dependency-service/photo-picker/) will teach you how to write a Dependency Service to fetch photos from Photo Library. For futher details: [link](https://developer.xamarin.com/guides/xamarin-forms/application-fundamentals/dependency-service/).

[//]: # (Links Section)
[xamarinWin]: <https://developer.xamarin.com/guides/android/getting_started/installation/windows/>
[xamarinStudioMac]: <https://developer.xamarin.com/guides/cross-platform/xamarin-studio/>
[xamarinVisualStudioMac]: <https://docs.microsoft.com/en-us/visualstudio/mac/installation>