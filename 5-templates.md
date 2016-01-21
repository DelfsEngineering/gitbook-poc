##Templates and Variables in Gitbook

There are conditional tags like **_if_**, **_elif_** (short for else if), **_else_**, **_for_** to evaluate text to be included based on the conditions or loop over an array. For example 

With 
{% raw %}
	{% if book.pocVariable %}
	  This text is being displayed since pocVariable == true
	{% endif %}
{% endraw %}

{% if book.pocVariable %}
This text is being displayed since pocVariable == true
{% endif %}

{% raw %}
	{% for person in book.teamPeople %}
		- {{person.name}}
	{% endfor %}
{% endraw %}

Returns a list of all names in the *teamPeople* array of objects. 

	{% for person in book.teamPeople %}
		- {{person.name}}
	{% endfor %}

My book.json looks like 

```javascript
{
    "styles": {
        "website": "styles/website.css"
    },

    "variables": {
        "pocVariable": true,
        "teamPeople":[
            { "name": "Rishabh" },
            { "name": "Arihant" },
            { "name": "Suvarna" },
            { "name": "Ashok" },
            { "name": "Pinky" },
            { "name": "Mayur" },
            { "name": "Anusheel"},
            { "name": "Vidhya" },
            { "name": "Abhraham"},
            { "name": "Shafeeq"},
            { "name": "Surbhi"}
        ]
    }
}
```

To access the *variables* in **book.json** we use *book.nameOfTheVariablePropertyInVariablesKey* (in this case **book.teamPeople**, and **book.pocVariable**)

###Inheriting 

You can also inherit template **blocks** (text templates) from one file to another. For example if in a hypothetic file named *mypage.md* I've the following markup written in it 

{% raw %}
    {% block pageContent %}
    This is the default content
    {% endblock %}
{% endraw %}

The **block** named *pageContent* can be imported in another file say named *mypage2.md* by writing 

{% raw %}
    {% extends "./mypage.md" %}

    {% block pageContent %}
    # This is my page content
    {% endblock %}
{% endraw %}