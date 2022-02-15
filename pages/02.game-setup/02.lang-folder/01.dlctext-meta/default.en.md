---
title: dlctext.meta
date: '02/13/2022 11:14'
---

## dlctext.meta File

### How to make a `dlctext.meta` file?
It's simple, make the file in the same place you have other meta files, usually `<RPF>/common/data`.
<br>Paste this code inside the file:
```xml
<?xml version="1.0" encoding="UTF-8"?>

<CExtraTextMetaFile>
	<hasGlobalTextFile value="true"/>
	<hasAdditionalText value="false"/>
	<isTitleUpdate value="false"/>
</CExtraTextMetaFile>
```
You need to reference the file in `content.xml`. This goes inside the `dataFiles` section
```xml
    <Item>
      <filename>dlc_NAME_GOES_HERE:/PATH_GOES_HERE/dlctext.meta</filename>
      <fileType>TEXTFILE_METAFILE</fileType>
      <overlay value="false" />
      <disabled value="true" />
      <persistent value="false" />
    </Item>
```
And put this inside the `filesToEnable` section
```
<Item>dlc_NAME_GOES_HERE:/PATH_GOES_HERE/dlctext.meta</Item>
```
! **Remember to change the `NAME_GOES_HERE`  and `PATH_GOES_HERE`!**