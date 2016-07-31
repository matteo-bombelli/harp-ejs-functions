# harp-ejs-functions

## IMPORTANT NOTE

This work is in **very early stage** or **pre-alpha**.

It doens't work for now (some scripts are not ended).

The reason for putting that online is to "inspire" and search for help maybe on this work.

## Im short

* **name** : Harp ejs functions
* **goal** : Easier creation and management of harp static websites
* **choices** : *EJS* templating/functions, *less* for style

## Indications 

All this features are made to be used with [harpjs](http://harpjs.com/) on top of [nodejs](https://nodejs.org/en/)

[here](http://harpjs.com/docs/quick-start) you can see also the install guide for harpjs

A list of functions to create a website in harp with more features using ejs templating engine.

## Goals

> **Use harp features and build functions to make websites creation easier and faster.**

Insted of writing tons of code directly in the template and repeat them 
when need I've choosen to create functions as properties of the object **MB**.
All the functions are divided by *categories* (or *libraries* ):

*   polyfills (like "shallow copy", getBasePath(to create standard websites that work in **GitHub Pages** ;) )
*   general;
*   file
*   number
*   post
*   date
*   number
*   locale (multilingual utilities);
*   frameworks (to better use partials);

All the system is extensible by creating new functions and categories. 
Adding files and elements to the `mbfunction.library` global array in harp.json will make 
theese function be loaded with the others in harp. 

The functions I've entered are mostly inspirated by my expirience with developing 
websites dynamically and statically. There are some functions that really remember 
other projects (like *wordpress*), but ported and adjusted to harp system.

For now the code is only partially comented and is something that i will work on 
more in the future.

As soon as possible I will create also a website and a wiki about this project.

**NOTE:**
If you need some functions in some pages and you know that they don't depend on others, 
you can put an `mbfunction.library` different array in some `_data.json` file, but 
remember to copy **all** the others values of the object (or indexed array ;) `mbfunction`

## Note on my choiches: EJS

Jade scares me cause it is harder for me to divide markups, content & script, 
so i will use **ejs**

## Thank YOU!

Please Fork and develop with me

And have fun while coding!

Matteo