# MOOC Index

One essential question is how abstract our framework will be.

On Wikiversity each page must exist in order to be browsed.
There is no way of capturing sub page request pointing to a page not existing yet.
Thus a central index that is aware of the MOOC and its content is not sufficient.

We could generate the code that has to be copied into a page created or
we might use the PHP API - unknown to me so far - to create this page with the generated code.
This must be done whenever the index changes in order to keep all pages up to date.

Just a thought: If this gets harder than expected an external software would solve this issue easily.

## Index content

The Index has to know the title of each MOOC item in order to name it.
This title will be the URL - if not set manually.

### Item
* title: String
* url: (opt) relative URL if not equal to ``wikiurl(title)``
