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

    title = "Testy"
    lunits = {}
    lunits[1] = "firstUnit"
    lunits[2] = "secondUnit"
    renderLesson(title, lunits)

If we are not allowed to execute code like this, we should try out if a module can keep a state within one page request or if the module looses it every time it gets called.
