
# بسم الله الرحمن الرحيم

# In the name of Allah, Most Gracious, Most Merciful

## Islamic-Speakers-Transcripts-and-Subtitles

### Folder and File Structure
```
root
├── Speaker Name
	├── laneguage (En)
    		├── Lecture Name 1
			└── Lecture Name_en.meta (Info about the lecture,Name, Date, Place etc)
			└── lecture Name_en.txt (Lecture text, utf-8 encoded)
			└── Lecture Name_en.srt (Subtitle)
			└── Lecture Name_en.odt (open document)
			└── Lecture Name_en.pdf (pdf file)
		├── Lecture Name 2
			~
		├── Lecture Name 3
			~
	├── Language (Bn)
		├── Lecture Name 1
			└── Lecture Name_bn.meta (Info about the lecture,Name, Date, Place etc)
			└── lecture Name_bn.txt (Lecture text, utf-8 encoded)
			└── Lecture Name_bn.odt (open document)
			└── Lecture Name_bn.pdf (pdf file)
			└── Lecture Name.srt (Subtitle)
		├── Lecture Name 2
			~
		├── Lecture Name 3
			~
```

<b>Note: Creating meta, txt and srt files are in higher priority</b>

#### Example Folder and file Structure
```
 root
 ├── Ahmed Deedat
    ├── En
        ├── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)
            └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_en.meta
            └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_en.txt
            └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_en.srt
            └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_en.odt
            └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_en.pdf
        ├── IS JESUS GOD
          ~
        ├── DEBATE - WAS CHRIST CRUCIFIED
          ~
    ├── Bn
      ├── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)
          └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_bn.meta
          └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_bn.txt
          └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_bn.srt
          └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_bn.odt
          └── WHAT THE BIBLE SAYS ABOUT MUHAMMAD (PBUH)_bn.pdf
          ├── IS JESUS GOD
            ~
          ├── DEBATE - WAS CHRIST CRUCIFIED
            ~
```
### Subtitling Guide:

http://bbc.github.io/subtitle-guidelines/

### Subtitling Free Tools:
* [SubtitleEdit](https://github.com/SubtitleEdit)
* Subtitle Workshop
* Subtitle Editor
* Open Subtitle Editor
* Aegisub
* [Google2srt](http://google2srt.sourceforge.net/en/)

### Source:
You can find most speakers in here: <a href="muslimcentral.com">muslimcentral.com</a>

## Text Cleanup
### Regex to remove html tags
```
<(?:[^>=]|='[^']*'|="[^"]*"|=[^'"][^\s>]*)*>
```
or
```
<[^>]*>([\s]?)*<[^>]*>
```
or
```
<(.|\n)+?>

```
### Regex to remove subtitle timestamps
```
([0-9]*\n([0-9]{2}:){2}[0-9]{2},[0-9]{3} --> ([0-9]{2}:){2}[0-9]{2},[0-9]{3})
```
