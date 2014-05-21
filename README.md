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
* **Quiz transclusion fails due to missing namespace** (fix: template has to be changed -> affects Topic:-quizzes => no fix, see below)
* **Parent transclusion fails due to missing namespace** (fix: template has to be changed -> affects Topic:-pages => fix after move completed)
* add script help text is wrong
* navigation is not aware of unset parameters
* no info text for missing video
* Talk: and /Quiz can be appended to a parameter pointing to template-using page automatically
* LUA: relative URLs? (relative to context=template-using page, such as /Quiz)

## Block (no template)
* custom block navigation
* no lesson navigation

## Lesson (no template)
* no lesson navigation

# Moved sites
**All URLs corrected** implies quiz is moved.

| Part | Block | Lesson | Learning Unit | Moved | All URLs corrected | missing parameters | notes |
| :--: | :---: | :----: | :-----------: | :---: | :----------------: | :----------------: | :---: |
| | Internet Architecture ||| Yes | No | no template | custom block navigation |
| || Ethernet || Yes | No | no template ||
| ||| COASM    | Yes | Yes | previous | OGV |
| ||| EH       | Yes | Yes | script | WEBM |
| ||| MPLvsMCL | Yes | Yes | script | WEBM |
| ||| CD       | Yes | Yes | script | OGV |
| ||| SFH      | Yes | Yes | video, script, next | |
| || Internet Protocol || Yes | No | no template ||
| ||| MFIP     | Yes | No | script, previous | WEBM |
| ||| CIPv4N   | Yes | No | script | WEBM |
| ||| IPFA     | Yes | No | script | WEBM |
| ||| IPH      | Yes | No | script | WEBM |
| ||| SFH      | Yes | No | video, script, next | |
