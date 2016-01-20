##Getting Started 

First page of the documentation/book is read through **README.md** file (in the root folder of the project). If the file is not present in the SUMMARY, it will be added as a first entry.[^2]

**SUMMARY.md** file maintains the index of all tree structure as you can see on the left side. The *SUMMARY.md* of this gitbook looks something like this : 
	# Summary

	* [Why Gitbook](1-WhyGitbook.md)
	* [Installing Github](2-InstallingGitbook.md)
	* [Getting Started](3-GettingStarted.md)

**GLOSSARY.md** : Allows you to specify terms and their respective definitions to be displayed in the glossary. Based on those terms, gitbook will automatically build an index and highlight those terms in pages. My Glossary.md looks like : 
	# Gitbook
	Is a book / document publishing tool

So when you click on *Gitbook* anywhere, you'll automatically taken to the full definition of the term *Gitbook* 



***

[^2]:Use another file than README.md for the introduction specify : 

```javascript
{
    "structure": {
        "readme": "myIntro.md"
    }
}
```

in the **book.json** file (placed in root folder)



