##Configurations and Plugins

>All configurations are stored as JSON in a file named **book.json**.

###Relevant Fields: 

* #####Gitbook Version:
```Javascript 
{ "gitbook": "2.x.x" } 
```
* #####Title : 
```Javascript 
{ "title": "My Awesome Book" }```

If not specified it is extracted from README.md (First Line)
* #####Description: 
```Javascript 
{ "description": "This is such a great book!" }```

If not specified it is extracted from README.md (First Paragraph)
* #####Styles: 
```Javascript 
{
    "styles": {
        "website": "styles/website.css",
        "ebook": "styles/ebook.css",
        "pdf": "styles/pdf.css",
        "mobi": "styles/mobi.css",
        "epub": "styles/epub.css"
    }
}
```

* #####Plugins :
```Javascript 
{ "plugins": ["mathjax"] } ```

Plugins can be searched and downloaded from [Plugins Site][1]

* #####Variables
```Javascript
{
    "variables": {
        "myTest": "Hello World"
    }
}
```

[1]: https://plugins.gitbook.com/

* #####Plugin Config : 
```Javascript
{
    "plugins": ["myplugin"],
    "pluginsConfig": {
        "myPlugin": {
            "message": "Hello World"
        }
    }
}
```
This option contains all plugin specific details

* #####Structure 
```Javascript 
{
    "structure": {
        "readme": "INTRO.md"
    }
}
```
