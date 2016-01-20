##Getting Started 

First page of the documentation/book is read through **README.md** file (in the root folder of the project). If the file is not present in the SUMMARY, it will be added as a first entry.[^2]

**SUMMARY.md** file maintains the index of all tree structure as you can see on the left side. The *SUMMARY.md* of this gitbook looks something like this : 
	# Summary

	* [Why Gitbook](1-WhyGitbook.md)
	* [Installing Gitbook](2-InstallingGitbook.md)
	* [Getting Started](3-GettingStarted.md)
	* [Making Sub Chapters](4-SubChapters.md)
		* [Sub Chapters Example 1](sub-chapters/1-subChapterExample.md)
		* [Sub Chapters Example 2](sub-chapters/2-subChapterExample.md)
		* [Sub Chapters Example 3](sub-chapters/3-subChapterExample.md)
	* [Templates and Variables in Gitbook](5-templates.md)
	* [Bringing Content from Other Files/Books](6-ContentReference.md)
	* [Configurations & Plugins](7-ConfsAndPlugs.md)
	* [Linking the Documentation on Github Page](8-ghPageIntegration.md)


**GLOSSARY.md** : Allows you to specify terms and their respective definitions/meanings to be displayed in the glossary. Based on those terms[I have specified only *Gitbook*], gitbook will automatically build an index and highlight those terms in pages. My Glossary.md looks like : 
	# Gitbook
	Is a book / document publishing tool

So when you click on *Gitbook* anywhere(but not in code), you'll automatically be taken to the full definition of the term *Gitbook* 


***

[^2]:To use another file than README.md for the introduction, specify : 

```javascript
{
    "structure": {
        "readme": "myIntro.md"
    }
}
```

in the **book.json** file (placed in root folder)



