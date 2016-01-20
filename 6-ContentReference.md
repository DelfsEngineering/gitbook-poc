##Bringing Content from Other Files/Books

##### Content referencing (conref) is a convenient mechanism for reuse of content from other files or books.

Include content from other files using 
{% raw %}
	{% include "/path_to_the_files" %}
{% endraw %}

For example I'll do

{% raw %}
	{% include "README.md" %}
{% endraw %} 

***
####README.md file in imported as a content.
{% include "README.md" %}
***

Content can also be included from other git book: [Link][1]

[1]: https://help.gitbook.com/format/conrefs.html

