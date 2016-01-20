##Why Gitbook?

Making Documentation with gitbooks is fast because 
1. It uses markdown
2. It can be configured
	- [Support for multiple languages][1]
	- Can be converted into Multiple Formats like PDF, ePub, Mobi, HTML
	- [Styles of the website][2] can be tailored and customized.
3. There's a concept of 'Variables' which are accessible through [templates][3]. 
4. There are also special tags like **_if_**, **_elif_**, **_for_** (short for else if) and **_else_** that can be used in the templates for {% if book.pocVariable %} selectively display the content. {% endif %}. 
5. Inbuilt javascript code and syntax highlighting for javascript
6. It has lots of plugins like disqus for commenting, to enhance its features

[1]: http://help.gitbook.com/format/languages.html
[2]: http://help.gitbook.com/styling/book.html
[3]: http://help.gitbook.com/format/templating.html