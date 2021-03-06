---
layout: post
title: MvvmForms Readme
permalink: new-page.html
description: Readme for Mvvm Forms
date: 2015-05-17 16:31:30 -07:00
tags: "MVVM; Windows Forms"
---

# MvvmForms ReadMeFirst!

Welcome to ActiveDevelop's MvvmForms Library Project. MvvmForm's purpose is to provide XAML ViewModel compatible support for Windows Forms Visual Basic and CSharp Projects and Solutions including a full-blown WinForms Designer support. MvvmForms is Open Source (GPL), but Dual License. For more Information about MvvmForms licensing read the License section below.

## Why Mvvm for WinForms? Does it make sense? Why not using WPF/XAML to begin with?

If you have the luxury of a clean start for your new project, and your development team is up to the task, you most probable do not need MvvmForms. But that is not that often the case. In most scenarios hundreds of millions of lines of code have been written for the Windows platform during the time between 1996 and 2010, and often in CSharp and Visual Basic .NET for Windows Forms, or even with Visual Basic 6. Many companies don't have the means of throwing those projects away and start from scratch. And what for, anyway? Your solution works, it is stable and tested. So, why not continue using it? 

MvvmForms is for you if you want to change your development paradigm. If you want to get rid of Code Behind and introduce a good architecture with separation of concerns. If you want to build based on an architecture which allows unit testing. If you want to create an multi-tier architecture from your existing software simply by refactoring part by part, where you can reuse big parts of the software for different UIs like for Windows Universal Apps, iOS Apps or Android Apps.

Our company, located in Westphalia Germany, has specialized in migrating from a typical Windows Forms Code Behind paradigm to a modern architecture. And we help to do this in a feasible way. We know, your team does neither have the time nor the budget to start from scratch, and that is the reason we developed MvvmForms: To help our customers to enter the new world of software development without jeopardizing the project.

## How does it work?

MvvmForms is a collection of controls for Windows Forms. Originally, it was designed to speed up the development process for data-heavy forms, and to address the need for database backends with their typical scenarios like zero-effort-handling of DBNulls, dirty-state handling of forms, focus highlighting, processing of formulas in numeric data entry fields, multi-threaded/multi-column lookup popups for collections up to 100.000 items, and much more. Sometime in mid-2012, a couple of German companies approached us to find a way to keep their existing Windows Forms design, yet they wanted to be able to apply the Mvvm pattern for parts of their LOB applications, so they could reuse this code in mobile apps and for other purposes. That was the start for MvvmForms, and we developed it from the existing toolset. This worked exceptional well, so we continued this approach and added rich designer functionality for the Mvvm components.

Because of this history, MvvmForms actually addresses two Windows Forms requirements. The first is to simplify designing data-heavy forms by providing controls like NullableDateValue, NullableNumValue, NullableTextValue, controls for DirtyState handling in Forms and so on.

The second one is to enable a Windows Forms for Mvvm. For this to end, you do not need to use one of the controls MvvmForms provide, you just need one component: the MvvmManager component. Basically, just drag that component into your form, set its DataContextType property to the type of the ViewModel, you want to bind, and every control on that form will get a PropertyBindings property which allow you to bind against the corresponding ViewModel property. You just need to set the DataContext property of the MvvmManager Component at runtime. You'll find a short step-by-step guide for getting started, read the wiki - the links is here on the right side.

On top: take a look at this introduction video on youtube, which does not only give an introduction to MvvmForms, but also to MVVM in general.

https://www.youtube.com/watch?v=1R_81Np5New

## How stable is MvvmForms? Have you done large LOB projects with it?

Oh, yes! Our team at ActiveDevelop is taking care of MvvmForms on a daily bases, because a couple of big projects in Germany rely on MvvmForms - some bigger than 1 Million lines of code. Since we are a German company, and we're started to localize MvvmForms to English, there are still a lot of German comments and XML-Docu-Tags inside the source - but we're working on it. But, MvvmForms is ready to be used, it is stable, reliable, thoroughly tested, and if you need special support or want to start with it urgently and need us to customize, localize or extend its functionality, than simply talk to us, so we can find a way to make this happen. 

## Can I use it both for CSharp and Visual Basic WinForms Projects?

Yes, with no limitations. A third of our current projects are in CSharp, the rest we do in VB, and parts of MvvmForms (the Mvvm Base Library for example) are in CSharp, as well. Other parts are in VB. So, as long as you do Windows Forms, your good to go - the language doesn't matter,

## So, MvvmForms is Open Source. Then, it's free, right?

Yes, for open source projects. For propriety, commercial projects, it's not entirely free, but also almost as good as free. Our primary goal is to find new opportunities to help with our 25+ year expertise in designing LOB Applications, and especially to show a way for our customers to migrate their software from being a big, monolithic Win32-Software to a modern approach without risk, where they can go forward with cloud computing, Windows 10, Mobile Apps, and all that without redoing everything from scratch.

So, if you want us to help you with your existing Application by doing workshops, helping with designing a new architecture, finding a feasible migration concept, introducing Scrum to your team, or providing human resources for a limited period of time for the purpose of the modernisation process, we bring MvvmForms along. Then it's free for you, because you're our customer. Go ahead and use it: You got an implicit licence for any commercial use, if you are or have been our customer at one point. If you, however, do not want us, but you want the toolset, just talk to us, and we figure out the best support model for you: mvvmforms@activedevelop.de.

If you're maintaining an open source project under GPL, and you want to use it. Go ahead: Fork it, change it modify it, and sell it along with your Open Source App. That's Open Source! As long your Application which links to it, or uses classes which derive from MvvmForms is also GPL - that is perfectly OK. But, if you're managing a propriety, close source solution, and you want to use (link to, derive from) MvvmForms, you have to obtain one license per active developer.

## Can I contribute?

Yes. Just create Pull Requests.
