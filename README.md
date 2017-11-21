
# بسم الله الرحمن الرحيم

# In the name of Allah, Most Gracious, Most Merciful

## Islamic-Sprekers-Transcripts-and-Subtitles

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
<(?:[^>=]|='[^']*'|="[^"]*"|=[^'"][^\s>]*)*>
or
<[^>]*>([\s]?)*<[^>]*>
### Regex to remove subtitle timestmap
([0-9]*\n([0-9]{2}:){2}[0-9]{2},[0-9]{3} --> ([0-9]{2}:){2}[0-9]{2},[0-9]{3})