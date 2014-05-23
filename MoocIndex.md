# MOOC Index

One essential question is how abstract our framework will be.

On Wikiversity each page must exist in order to be browsed.
There is no way of capturing sub page requests pointing to a page not existing yet.
Thus a central index that is aware of the MOOC and its content is not sufficient: We have to create pages.

We could generate the code that has to be copied into the page for a new MOOC item or
we might use the PHP API - unknown to me so far - to create this page with the generated code.
This must be done whenever the index changes in order to keep all pages up to date.  
(If this gets harder than expected an external software would solve this issue easily.)

## Index content

The Index has to know the title of each MOOC item in order to name it.
This title will be the URL - if not set manually.

#### Learning Goals (Learning Unit)

At the moment these are only existing and shown in the parental table.
We could easily move them to the learning unit and transclude them. We could also use a sub page just like for scripts and quizzes.
Both ways enable us to show them in the learning unit, too.

