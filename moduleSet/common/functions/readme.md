# functions Root

	/moduleSet/common/functions/

this is the path where remain the core of the functions. This path is defined into the `mbfunction.path` value into `harp.json` `globals`, the global values avaibles for all the pages (and the functions).

## usage in harp.

harp gives you the possibility to use partials and ejs gives you the possibility 
to use some scripting into the template.

to add the functions to a template, a module, a layout or an ejs page you need to add to 
the top (or before using the functions) the line

```EJS
<% 
pathToPublicRoot = "../"; // this is just an example if you are in the public folder this is just "" 
partial(pathToPublicRoot + mbfunctions.path) 
%>
```

this will load the functions and make them available for you.

the property `mbfunctions.path`, that I prefer to add to the 
[globals of harp.json](https://harpjs.com/docs/development/globals), 
define the path of the function ejs file relative to the root of the `public` path;

## libraries

The libraries are placed into the `lib` subfolder. There you can find the core 
functions divided in files based on categories.

The list of the categories/files you want to load is defined in the 
`mbfunctions.libraries` variable, also in harp.json globals.

If you want to develop your functions you can add files to lib folder 
and add the files names to the libraries property.

**IMPORTANT NOTE**:
all the defaults libraries are not indipendent so removing them can create 
problems.