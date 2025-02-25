---
search:
  boost: 0.5
title: SAYFILES
---

# SAYFILES()

### Synopsis

Returns the ampersand-delimited file names that would be played by the Say applications (e.g. SayAlpha, SayDigits).

### Since

16.21.0, 18.7.0, 19.0.0

### Description

Returns the files that would be played by a Say application. These filenames could then be passed directly into Playback, BackGround, Read, Queue, or any application which supports playback of multiple ampersand-delimited files.<br>

``` title="Example: Read using the number 123"

same => n,Read(response,${SAYFILES(123,number)})


```

### Syntax


```

SAYFILES(value,type)
```
##### Arguments


* `value` - The value to be translated to filenames.<br>

* `type` - Say application type.<br>

    * `alpha` - Files played by SayAlpha(). Default if none is specified.<br>

    * `digits` - Files played by SayDigits().<br>

    * `money` - Files played by SayMoney(). Currently supported for English and US dollars only.<br>

    * `number` - Files played by SayNumber(). Currently supported for English only.<br>

    * `ordinal` - Files played by SayOrdinal(). Currently supported for English only.<br>

    * `phonetic` - Files played by SayPhonetic().<br>

### See Also

* [Dialplan Applications SayAlpha](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/SayAlpha)
* [Dialplan Applications SayDigits](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/SayDigits)
* [Dialplan Applications SayMoney](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/SayMoney)
* [Dialplan Applications SayNumber](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/SayNumber)
* [Dialplan Applications SayOrdinal](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/SayOrdinal)
* [Dialplan Applications SayPhonetic](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/SayPhonetic)


### Generated Version

This documentation was generated from Asterisk branch 16 using version GIT 