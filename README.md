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
* **Quiz transclusion fails due to missing namespace** (fix: template has to be changed -> affects Topic:-quizzes => no fix, see below)
* **Parent transclusion fails due to missing namespace** (fix: template has to be changed -> affects Topic:-pages => fix after move completed)
* add script help text is wrong
* navigation is not aware of unset parameters
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

# Moved sites
**All URLs corrected** implies quiz is moved.

| Part | Block | Lesson | Learning Unit | Moved | All URLs corrected | missing parameters | notes |
| :--: | :---: | :----: | :-----------: | :---: | :----------------: | :----------------: | :---: |
| | Internet Architecture ||| Yes | Yes | no template | custom block navigation |
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
| ||| pn | Yes | Yes | script | WEBM "Portnumbers" -> "Port_Numbers" |
| ||| swafp | Yes | Yes | script | WEBM "slidingwindow" -> "Sliding Window and Flow Control" |
| ||| SFH | Yes | Yes | video, script, next | |
| || DNS || Yes | No | no template | |
| ||| TS | Yes | No | script, previous | WEBM |
| ||| T | Yes | No | script | WEBM |
| ||| Z | Yes | No | script | WEBM |
| ||| RsfaDNS | Yes | No | script | WEBM |
| ||| DDNSQ | Yes | No | script | WEBM |
| ||| DNSAR | Yes | No | script | WEBM "DNS address resolution" -> "DNS Address Resolution" |
| ||| SFH | Yes | No | script, next | WEBM |
| | Web Architecture ||| Yes | No | no template | **no children** |
