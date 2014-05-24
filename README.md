# Templates

## Learning Unit (depreceated: Lesson)
* title (fulltext)
* video (File:filename)
* script (fulltext)
* quiz (URL /Quiz) CAN BE CUT
* talk (URL Topic_talk:) MUST BE EDITED
* furtherReading (fulltext)
* parent (URL)
* next (URL)

**notes**:
* **template not moved** yet
* add script help text is wrong
* template is not aware of unset parameters
* no info text for missing video
* Talk: and /Quiz can be appended to a parameter pointing to template-using page automatically
* LUA: relative URLs? (relative to context=template-using page, such as /Quiz)

## Block (no template)
* no lesson navigation
* custom block navigation

## Lesson (no template)
* **category not changed** yet to have all in same category => fix after move completed
* no lesson navigation
* table with learning units (transcluded by learning units)
* lesson video

# Fixes

## Learning Unit (depreceated: lesson)
* script transclusion fixed with LUA
  
  pseudocode: ``if (script.startsWith('Web_Science')) transclude(:script) else print(script)``

* quiz transclusion fixed with LUA

  pseudocode: ``if (quiz.startsWith('Web_Science')) transclude(:quiz) else transclude(quiz)``

* parent transclusion fixed with LUA

  pseudocode: ``if (parent.startsWith('Web_Science')) transclude(:parent) else transclude(parent)``

# Todo
after all MOOC items are moved:
* short look at Module:Lesson
* test transclusion behaviour of {{talkpagenamee}}
* create transclusion diagram
* move templates (?)
* rebuild templates
* use new template URLs in MOOC items

# Moved sites
**All URLs corrected** implies quiz is moved.
It also implies script is moved for lesson "Web Content" and later.

| Pages                       | Moved | Updated | notes |
| :-------------------------: | :---: | :-----: | :---: |
| __root__ | Yes | Yes | |
| Part1: Foundations of the web | Yes | Yes | still linking to outdated Web History not moved yet |
| Part2: Emerging Web Properties | Yes | Yes | very large: aggregates 3 of 5 subpages |
| Part3: Web & Society | Yes | Yes | mv "Part3: Web & society"; only page of the part |
| Flipped Classroom | Yes | Yes | mv "Flipped classroom" |
| Enrole | Yes | Yes | |
| New here | Yes | Yes | |
| Web Architecture and Web History | No | No | outdated; not moved |
| All learning units talk | Yes | No | |
| current learning units talk | Yes | Yes | |

## [Part] #1

| Block                       | Moved | Updated | notes |
| :-------------------------: | :---: | :-----: | :---: |
| Internet Architecture       | Yes   | Yes     | |
| Internet vs. world wide web | Yes   | No      | |
| Web Architecture            | Yes   | Yes     | no block navigation |

### [Block] Internet Architecture

| Lesson                        | Moved | Updated | notes |
| :---------------------------: | :---: | :-----: | :---: |
| Ethernet                      | Yes   | Yes     | |
| Internet Protocol             | Yes   | Yes     | current discussions link (page bottom) |
| Transmission Control Protocol | Yes   | Yes     | |
| Domain Name System            | Yes   | Yes     | |

#### [Lesson] Ethernet

| Learning Unit                                  | Moved | Updated | missing parameters  | notes |
| :--------------------------------------------: | :---: | :-----: | :-----------------: | :---: |
| Communication over a shared Medium             | Yes   | Yes     | previous            | OGV |
| Ethernet Header                                | Yes   | Yes     | script              | WEBM |
| Minimum Package length vs Maximum cable length | Yes   | Yes     | script              | WEBM |
| Collision Detection                            | Yes   | Yes     | script              | OGV |
| SFrH                                           | Yes   | Yes     | video, script, next | |

#### [Lesson] Internet Protocol

| Learning Unit           | Moved | Updated | missing parameters  | notes |
| :---------------------: | :---: | :-----: | :-----------------: | :---: |
| Motivation for IP       | Yes   | Yes     | script, previous    | WEBM |
| Classfull IPv4 networks | Yes   | Yes     | script              | WEBM |
| IP forwarding algorithm | Yes   | Yes     | script              | WEBM |
| IP header               | Yes   | Yes     | script              | WEBM |
| SFrH                    | Yes   | Yes     | video, script, next | |

#### [Lesson] Transmission Control Protocol

| Learning Unit                                              | Moved | Updated | missing parameters  | notes |
| :--------------------------------------------------------: | :---: | :-----: | :-----------------: | :---: |
| End to End Principle and Connection oriented Communication | Yes   | Yes     | script, previous    | WEBM |
| 3 way handshake                                            | Yes   | Yes     | script              | WEBM |
| Port Numbers                                               | Yes   | Yes     | script              | WEBM; mv "Portnumbers" |
| Sliding Window and Flow Control                            | Yes   | Yes     | script              | WEBM; mv "slidingwindow" |
| SFrH                                                       | Yes   | Yes     | video, script, next | |

#### [Lesson] Domain Name System

| Learning Unit               | Moved | Updated | missing parameters | notes |
| :-------------------------: | :---: | :-----: | :----------------: | :---: |
| Tree Structure              | Yes   | Yes     | script, previous   | WEBM |
| Terminology                 | Yes   | Yes     | script             | WEBM |
| Zones                       | Yes   | Yes     | script             | WEBM |
| Review some facts about DNS | Yes   | Yes     | script             | WEBM |
| Delegating DNS Queries      | Yes   | Yes     | script             | WEBM |
| DNS Address Resolution      | Yes   | Yes     | script             | WEBM; mv "DNS address resolution" |
| SFrH                        | Yes   | Yes     | script, quiz, next | WEBM; /table moved |

### [Block] Web Architecture

| Lesson                      | Moved | Updated | notes |
| :-------------------------: | :---: | :-----: | :---: |
| Hypertext Transfer Protocol | Yes   | Yes     | mv "Hypertext transfer protocol" |
| Web Content                 | Yes   | Yes     | resources navigation column is introduced here; wget script; /Markup_Languages not moved |
| Dynamic Web Content         | Yes   | Yes     | |

#### [Lesson] Hypertext Transfer Protocol

| Learning Unit        | Moved | Updated | missing parameters | notes |
| :------------------: | :---: | :-----: | :----------------: | :---: |
| Making HTTP requests | Yes   | Yes     | previous           | WEBM |
| A Simple Web Client  | Yes   | Yes     |                    | WEBM; title diff |
| A Simple Web Server  | Yes   | Yes     | quiz               | WEBM; empty quiz @ [...]Simiple[...]/Quiz; large script |
| The HTTP Header      | Yes   | Yes     | script             | WEBM |
| Content negotiation  | Yes   | Yes     |                    | WEBM |
| SFrH                 | Yes   | Yes     | script, next       | WEBM; script headline in further readings |

#### [Lesson] Web Content

| Learning Unit                               | Moved | Updated | missing parameters       | notes |
| :-----------------------------------------: | :---: | :-----: | :----------------------: | :---: |
| Problem Setting for Web Content Formats     | Yes   | Yes     | previous, furtherReading | WEBM; script transclusion from /Script is introduced here |
| Working with XML                            | Yes   | Yes     | furtherReading           | WEBM; video has 640px parameter; furtherReading in /Script |
| HTML for Web Document Structures            | Yes   | Yes     |                          | WEBM; mv "HTML for Web document structures" |
| Layout Elements in HTML                     | Yes   | Yes     | furtherReading           | WEBM |
| Motivating Separation of Content and Layout | Yes   | Yes     | quiz, furtherReading     | WEBM; empty quiz @ /Quiz not moved |
| Cascading Stylesheets (CSS)                 | Yes   | Yes     | furtherReading           | WEBM; mv "Lesson on Cascading Stylesheets (CSS)" |
| Media Content                               | Yes   | Yes     | quiz                     | WEBM; empty quiz @ /Quiz not moved |
| Metadata                                    | Yes   | Yes     | quiz, furtherReading     | WEBM |
| SFrH                                        | Yes   | Yes     | video, script, next      | |

#### [Lesson] Dynamic Web Content

| Learning Unit                             | Moved | Updated | missing parameters                 | notes |
| :---------------------------------------: | :---: | :-----: | :--------------------------------: | :---: |
| Basics of server side web programming     | Yes   | Yes     | previous                           | WEBM; {{talkpagename}}, /Quiz, {{/Script}} are introduced here |
| Forms and HTTP Post Request               | Yes   | Yes     | furtherReading                     | WEBM; mv "Forms and HTTP Post request" title diff |
| Handling a Post Request in a Java Servlet | Yes   | Yes     | furtherReading                     | WEBM |
| Client side JavaScript                    | Yes   | Yes     | furtherReading                     | WEBM; mv "Client side Javascript" |
| Ajax and the XMLHttpRequest Class         | Yes   | Yes     |                                    | WEBM |
| SFrH                                      | Yes   | Yes     | next, script, quiz, furtherReading | WEBM; **wrong video** |

## [Part] #2

| Block                       | Moved | Updated | notes |
| :-------------------------: | :---: | :-----: | :---: |
| Emerging Structure of the Web | Yes | Yes | |
| Search Engine Ecosystem | Yes | Yes | |
| Ranking | Yes | Yes | |
| Collective Intelligence | Yes | Yes | mv "Collective intelligence" |
| Online Communities | Yes | Yes | video only |

