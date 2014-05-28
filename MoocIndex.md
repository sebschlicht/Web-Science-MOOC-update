# MOOC Index

On Wikiversity each page must exist in order to be browsed.
There is no way of capturing sub page requests pointing to a page not existing yet.
Thus a central index that is aware of the MOOC and its content is not sufficient: We have to create pages.

These pages point to one MOOC item each, that gets rendered.

The MOOC Index is a central page holding the structure of the MOOC and some meta information.
The syntax is still in development and it is not clear what information has to be provided yet.

Since an item in the MOOC can have one of the following types its type hast to be provided together with the page title at least.

## Item types

| Type          | Identifier   | Short identifier |
| :-----------: | :----------: | :--------------: |
| lesson        | lesson       | l |
| learning unit | learningUnit | u |

There will be a bot one can trigger for a MOOC that will create a page for each MOOC item the index contains.

## Syntax

The index syntax will use Wikitext to make the index page readable.
A MOOC item looks like this:

    =lesson|Testy=

To increase the level and specify subpages act like in Wikitext - increase the number of `=`:

    =lesson|Testy=
    ==u|Unit1==
    ==learningUnit|Unit2==
    ==u|Unit3==

If there are additional parameters for an item you can provide them using a single line

    =lesson|Testy=
    *parameter=value

or multiple lines - recommended for muti-line values that use Wikitext syntax itself:

    =lesson|Testy=
    *parameter
    multiLineValue

An example is [LearningGoals](#LearningGoals).

 
Please note that each additional line of a value **must not** start with `*`, no matter which one of the two methods you use.

## Content

#### Learning Goals

Learning goals of the MOOC item can be set using the `learningGoals` parameter.
Separate single learning goals using `#`:

    =lesson|Testy=
    *learningGoals
    #goal1
    #goal2

