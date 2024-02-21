# JSCtoXML
## Forked from pkg10.17.0

Huge thanks to the @3DGISKing for the original modifications. The original repo had some problems, which 
are to be addressed in this fork:
- It wasn't clear which version of the v8 engine was modified - the closest one I could find is build [6.8.290](https://github.com/v8/v8/releases/tag/6.8.290)
- There was no patch, instead you were supposed to replace files - now we have a patch to apply against v8 project. I removed all unrelated changes (e.g. caused by auto-formatting), some [additional work](#note-on-modified-code) was done above that
- It's still not exactly clear how to use the provided code
- Original repo was published in early 2021, however the v8 build it was built upon dates back to mid 2018. In other words, it's completely outdated.

PRs and suggestions are very much welcome.
  

### Note on modified code
- `objects.h` didn't include changes from [this commit](https://github.com/v8/v8/commit/11aaf0fb84f979a4f09e63c65f500350e053e221#diff-3a388106f384db09426fc3a25392bf0a1cc7ead81045ee62b40f94c3ee405a95) that belongs to build [6.8.199](https://github.com/v8/v8/releases/tag/6.8.199)
- `objects.cc` included changes from [this commit](https://github.com/v8/v8/commit/d5686a74d56fbb6985b22663ddadd66eb7b91519#diff-d27f7e8788adb680270271c52e086d7adf00f2b127a5378062e45af7801b1db4) that belongs to build [6.9.405](https://github.com/v8/v8/releases/tag/6.9.405)

The reasons behind that are unclear and everything was synchronized to work with build [6.8.290](https://github.com/v8/v8/releases/tag/6.8.290) as a baseline

## OG repo video demonstration

[![](http://img.youtube.com/vi/cKU5tkZqomE/0.jpg)](http://www.youtube.com/watch?v=cKU5tkZqomE "")
