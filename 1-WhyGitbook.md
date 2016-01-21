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
6. It has lots of plugins like disqus for commenting, to enhance its features: like codepen integration, ace editor plugin
7. People can send pull requests for any discrepancy they have fixed/found in the documentation.
8. There's a search plugin for Gitbook, which can be used to look up for keyword search in the documentation.
[1]: http://help.gitbook.com/format/languages.html
[2]: http://help.gitbook.com/styling/book.html
[3]: http://help.gitbook.com/format/templating.html


####GOTCHAS
Right now, I haven't known if there's a way to automate gitbook documentation with or like JSDoc, as soon as I find a way, I'll update it.