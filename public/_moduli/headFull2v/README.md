# Guide for the headFull2v module

## head module

include it in your page at the top inside your html tag

uses this variables:

```JSON

    {
        "uri":"your-uri", // the uri of your site 
        "BasePath":"",
        "BaseUrl":"",
        "crossDomain":true, // can be true or false
        "AutoreArticoli":{
            "nome":"Your Name",
            "facebookPage":"https://www.facebook.com/your-fb-page/",
            "GooglePlusPage":"https://plus.google.com/your-gplus-profile",
            "twitterID":"@your-tw-ID"
        },
        "logoSito":{ // the logo of your site displayed by 
            "relUrl":true,
            "url":"", // the url for the image of your website
            "width":"", // the width of the image
            "height":"" //
        },
        "Publisher":{ // variables for the publisher data
            "nome":"Publisher Name", 
            "facebookPage":"[https://www.facebook.com/publisher-fb-page/]",
            "GooglePlusPage":"[https://plus.google.com/publisher-gplus-profile]",
            "twitterID":"[@publisher-tw-ID]"
        },
        "Thumb":{
            "url":"", 
            "relUrl":true,
            "width":"",
            "height":""
        }
    }

```

## Socials



### Socials Images specs

twitter:

*   **max filesize: 1MB**

*   min 280x150
 
*   max displayed: 1024x512

facebook:

*   imagesize: 1200 x 630;

*   min 200 x 200