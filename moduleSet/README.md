# Modules root

	/moduleSet

I've decided to create this place to put sources of the modular part of 
development to not create confusion in the public folder 

Here you can put **pages templates** and **modules** (partials). This components are 
grouped into `frameworks`.

## Folder hierarchy

Assuming this ( `moduleSet` ) as a **frameworks root** , the standard path for frameworks is like that:

* **moduleSet**
	* **framework-name** (folder)
		* **modules** (folder)
			* **module-name** (modules folder)
				* **module-name.ejs** (main file)
				* other-partials (requested by the main file)
				* main-module-style.less (if needed)
				* other-style (if needed)
			* **module-name-2** (folder)
				* **module-name-2.ejs** (main file)
				* ... etc.
		* templates (folder for page templates)
			* template-name (folder)
				* template-name.ejs (main template file)
				* ... etc. (just like modules) 

**LEGEND** :

* **bold** : *required*
* not bold : optional

## common framework

By standard I've inserted a `common` framework that will contain the common 
modules and eventually the common page templates so that it is easy to create a 
bootstrap for others developments.

`common` framework has also the function folder that contains functions and libraries.

[more detail on this part on this path](common/functions/);

## files types
This folder is not accessible from the web page directly, so it is important to not put 
here files like bitmap images that need to be linked in the page (you can put svg because 
you can use them in partials).

### in short terms:

usefull FILES in this folder:
*	ejs (can be used as partial for html, svg, txt ... everytype of file that is a text file, but remember that js files cannot be named js, but you can name them .jscript ;) )
*	less (you need to import them in main less file, see *less files* section)
*	md (you need to use them as partials or use them as wiki or description like *this one*)

Visible just in sources:
*	jpg, png, gif, and other images files
*	fonts
*	all binary files
