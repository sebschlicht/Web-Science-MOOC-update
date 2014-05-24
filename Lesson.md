# Lesson

A lesson has a name.  
It has learning goals to specify what is its intention.  
It can have a video explaining the content.  
It has one or more learning units being more specific learning items.

## Module

We could easily write a LUA module that would generate the lesson page.  
The learning unit names would be passed in a table.  
Video and learning goals would be simply transcluded to minify LUA usage.

### Usage

Ideal usage would be to execute code in the wiki page like this:

    title = "Testy"
    lunits = {}
    lunits[1] = "firstUnit"
    lunits[2] = "secondUnit"
    renderLesson(title, lunits)

Unfortunately we are not allowed to execute code outside of a module.  
We are not even able to store a variable in the module within a page request, every call creates a new module instance.
If we can not store the state in LUA we have to store it somewhere else.
There are three ways to overcome this issue.

#### Own Format

I did not find any way to handle a variable number of arguments, such as passing a table as show above.
Instead we could pass the **units in CSV** style using one argument to pass as many as needed.  
A more complex format to pass whole objects is also possible, to provide URL and video if not matching standard conventions.

**Example**

    {{#invoke:Lesson|render|myLesson|unit1,unit2,unit3}}

**pro**:
* one module call
* works without an index

**con**:
* does not work with index
* complex call if passing whole objects

#### Page

The wiki page could save the state for us.  
We would make mutliple module calls where each calls renders one particular learning unit.

**Example**

    {{#invoke:Lesson|printHeader|myLesson}}
    {{#invoke:Lesson|printUnit|unit1}}
    {{#invoke:Lesson|printUnit|unit2}}
    {{#invoke:Lesson|printUnit|unit3}}
    {{#invoke:Lesson|printFooter|myLesson}}

**pro**:
* very readable, even if passing whole objects
* works without an index

**con**:
* does not work with index
* multiple module calls, maybe partially with the same arguments

#### Index

One wiki page storing an index could save the MOOC structure and get accessed by all MOOC modules.

**Example**
page:

    {{#invoke:Lesson|render|indexUrl|myLesson}}

index:

    --MOOC-Index
    lesson_#|#_myLesson
      unit_#|#_unit1
      unit_#|#_unit2
      unit_#|#_unit3

**pro**:
* one module call
* minimal code

**con**:
* not clear if possible yet
* additional page request to access index

probably the best method to choose  
note: e.g. Lesson/Web_Science can be used for custom lesson modules

