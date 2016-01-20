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
            { "name": "Shafique"},
            { "name": "Surbhi"}
        ]
    }
}
```

To access the *variables* in **book.json** we use *book.nameOfTheVariablePropertyInVariablesKey* (in this case **book.teamPeople**, and **book.pocVariable**)
