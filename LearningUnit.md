# Learning Unit

A Learning Unit has a name.  
It has learning goals to specify what is its intention.  
It can have a video explaining the content.  
It can have one or more scripts providing material necessary. (-> user generated allowed?)  
It can have a quiz to enable users to test theirselves.  
It can have further reading to teach yourself beyond the boundary of the learning unit.  
It has a discussion page to ask questions. (-> separate page? talk page is rather for Wikiversity internal communication concerning page status than for questions of understanding)


## LearningGoals

At the moment learning goals are visible in the lesson table only.

## Video

URL: ``File:name.ext`` (could be generated if not passed as parameter using name and default video extension)  
is included in parental lesson: possible via transclusion

## Script

URL: ``learningUnit/Script``  
does not need to be included anywhere else  
a link asking for creation should be visible if not existing yet

## Quiz

URL: ``learningUnit/Quiz``  
does not need to be included anywhere else  
a link asking for creation should be visible if not existing yet

## FurtherReading

no separate page at the moment  
does not need to be included anywhere else  
no link can be provided: is template parameter (neither page nor section)

## Discussion

URL: {{TALKPAGENAME}} / {{TALKNAMESPACE}}:learningUnit  
does not need to be included anywhere else  
menu to ask a new question / reply to a specific question (may be possible by rendering page with LUA)

