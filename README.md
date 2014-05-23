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
* **template not moved yet**
* **Parent transclusion fails due to missing namespace** (fix: template has to be changed -> affects Topic:-pages => fix after move completed)
* **discussion menu is not working with {{talkpagename}}**
* add script help text is wrong
* template is not aware of unset parameters
* no info text for missing video
* Talk: and /Quiz can be appended to a parameter pointing to template-using page automatically
* LUA: relative URLs? (relative to context=template-using page, such as /Quiz)

## Block (no template)
* no lesson navigation
* custom block navigation

## Lesson (no template)
* **category** not changed yet to have all in same category => fix after move completed
* no lesson navigation
* table with learning units (transcluded by learning units)
* lesson video

# Fixes

## Learning Unit (depreceated: lesson)
* script transclusion fixed with LUA
  
  pseudocode: ``if (script.startsWith('Web_Science')) transclude(:script) else print(script)``

* quiz transclusion fixed with LUA

  pseudocode: ``if (quiz.startsWith('Web_Science')) transclude(:quiz) else transclude(quiz)``

# Todo
after all MOOC items are moved:
* short look at Module:Lesson
* test transclusion behaviour of {{talkpagename}}
* create transclusion diagram
* move templates (?)
* rebuild templates
* use new template URLs in MOOC items

# Moved sites
**All URLs corrected** implies quiz is moved.
It also implies script is moved for lesson "Web Content" and later.

| Part | Block | Lesson | Learning Unit | Moved | All URLs corrected | missing parameters | notes |
| :--: | :---: | :----: | :-----------: | :---: | :----------------: | :----------------: | :---: |
| | Internet Architecture ||| Yes | Yes | no template | |
| || Ethernet || Yes | Yes | no template ||
| ||| COASM    | Yes | Yes | previous | OGV |
| ||| EH       | Yes | Yes | script | WEBM |
| ||| MPLvsMCL | Yes | Yes | script | WEBM |
| ||| CD       | Yes | Yes | script | OGV |
| ||| SFH      | Yes | Yes | video, script, next | |
| || Internet Protocol || Yes | Yes | no template | current discussions link (page bottom) |
| ||| MFIP     | Yes | Yes | script, previous | WEBM |
| ||| CIPv4N   | Yes | Yes | script | WEBM |
| ||| IPFA     | Yes | Yes | script | WEBM |
| ||| IPH      | Yes | Yes | script | WEBM |
| ||| SFH      | Yes | Yes | video, script, next | |
| || TCP || Yes | Yes | no template | |
| ||| EtEPaCoC | Yes | Yes | script, previous | WEBM |
| ||| 3wh | Yes | Yes | script | WEBM |
| ||| Port Numbers | Yes | Yes | script | WEBM mv "Portnumbers" |
| ||| Sliding Windows and Flow Control | Yes | Yes | script | WEBM mv "slidingwindow" |
| ||| SFH | Yes | Yes | video, script, next | |
| || DNS || Yes | Yes | no template | |
| ||| TS | Yes | Yes | script, previous | WEBM |
| ||| T | Yes | Yes | script | WEBM |
| ||| Z | Yes | Yes | script | WEBM |
| ||| RsfaDNS | Yes | Yes | script | WEBM |
| ||| DDNSQ | Yes | Yes | script | WEBM |
| ||| DNSAR | Yes | Yes | script | WEBM mv "DNS address resolution" |
| ||| SFH | Yes | Yes | script, quiz, next | WEBM, /table |
| | Internet vs. world wide web ||| Yes | No | no template | |
| | Web Architecture ||| Yes | No | no template | |
| || Hypertext Transfer Protocol || Yes | Yes | | mv "Hypertext transfer protocol" |
| ||| MHTTPr | Yes | Yes | previous | WEBM |
| ||| ASWC | Yes | Yes | | WEBM title diff |
| ||| ASWS | Yes | Yes | quiz | WEBM empty quiz @ [...]Simiple[...]/Quiz; large script |
| ||| THTTPH | Yes | Yes | script | WEBM |
| ||| Cn | Yes | Yes | | WEBM |
| ||| SFH | Yes | Yes | script, next | WEBM script headine in further readings |
| || Web Content || Yes | Yes | no template | resources navigation column is introduced here; wget script; /Markup_Languages (unmoved) |
| ||| Problem Setting for Web Content Formats | Yes | Yes | previous, furtherReading | WEBM script transclusion from /Script is introduced here |
| ||| Working with XML | Yes | Yes | furtherReading | WEBM video has 640px parameter; furtherReading in /Script |
| ||| HTML for Web Document Structures | Yes | Yes | | WEBM mv "HTML for Web document structures" |
| ||| Layout Elements in HTML | Yes | Yes | furtherReading | WEBM |
| ||| Motivating Separation of Content and Layout | Yes | Yes | quiz, furtherReading | WEBM empty quiz @ /Quiz |
| ||| Cascading Stylesheets (CSS) | Yes | Yes | furtherReading | WEBM mv "Lesson on Cascading Stylesheets (CSS)" |
| ||| Media Content | Yes | Yes | quiz | WEBM empty quiz @ /Quiz |
| ||| Metadata | Yes | Yes | quiz, furtherReading | WEBM |
| ||| SFrH | Yes | Yes | video, script, next | |
| || Dynamic Web Content || Yes | Yes | no template | |
| ||| Basics of server side web programming | Yes | Yes | previous | WEBM {{talkpagename}} /Quiz {{/Script}} are introduced here |
| ||| Forms and HTTP Post Request| Yes | Yes | furtherReading | WEBM mv "Forms and HTTP Post request" title diff |
| ||| Handling a Post Request in a Java Servlet | Yes | Yes | furtherReading | WEBM |
| ||| Client side JavaScript | Yes | Yes | furtherReading | WEBM mv "Client side Javascript" |
| ||| Ajax and the XMLHttpRequest Class | Yes | Yes | | WEBM |
| ||| SFrH | Yes | Yes | next, script, quiz, furtherReading | WEBM **wrong video** |
