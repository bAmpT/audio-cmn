
**Audio-cmn** aims to provide hight quality & easy to use Chinese words audio recordings for modern web & mobile application. Audio-cmn is all
* an original work by the recording of chinese syllabs
* a curation work reusing pre-existing audios from SWAC Recorder
* a post-processing work by providing light & optimised `.mp3` files rather than the huge original `.flac` files.
These audios are thus suitable for mobile application developments.

### Voices
| # of items | Naming          | Set's specifics | Authorship |
| :--------- |:---------------:|:----------------|:-----------|
| 1707       | `cmn-zi4.mp3`   | syllabs v0.1    | Chen Wang, CC-by-sa |
| +8000      | `cmn-名字.mp3`   | HSK 2000 list (words,zi)  | Yue Tan, [CC-by-sa](http://packs.shtooka.net/cmn-caen-tan/readme.txt) |

### Project's structure
All audios exist in both 64kbts and 18-abr-kbts versions, each spliting between HSK words, HSK single characters, and Chinese syllabs.

* **/64k/** - optimal audio quality for voice recording.
  * /64k/syllabs -- all chinese syllabs (1707)
  * /64k/hsk/ -- HSK_2000, all zi and words (8,596)
* **18k-abr** - files are optimized, ~3 times lighter, for 80% of the audio quality.
  * /18k-abr/syllabs -- all chinese syllabs (1707)
  * /18k-abr/hskzi/ -- HSK_2000, all zi (1,735)
  * /18k-abr/hsk/ -- HSK_2000, all words (6,863)

### Missing audios ?
The current HSK audio database was build upon the official `HSK 2000`, published in 2000. The HSK 2000 is thus near fully covered (at least 8596 out of ~8800). List comparison with the last `HSK 2012` words list is available and done via :

```bash
bash ./missing-audios.bash  HSK2012_all.txt    # List missing audios, compared to input list of words
bash ./missing-audios.bash --help              # Tiny manual
```

Current difference: [582 HSK2012 words which are missing human audios](http://jsfiddle.net/fduyws3x/2/). See files in `./lists/` .

### Credits
* Speakers -- see table upper
* [Hugo Lopez](http://github.com/hugolpz), PLIDAM, INALCO -- Project management, repository, audio compression, file renaming
* Nicolas Vion -- recording software & technical support

### Log
* v.0.1.0: clean up data by deleting the cmn-*5.ext items
* v.0.1.1: add ./18k-abr (<40MB), an optimized version of ./64kb with almost equal sound quality
* v.0.1.2: improve README.md ; Add ./lists/ and script for comparison with the HSK2012.

### License
* CC-by-sa. See table upper for authors.
