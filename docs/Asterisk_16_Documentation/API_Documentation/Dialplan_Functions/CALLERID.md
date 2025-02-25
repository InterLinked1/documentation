---
search:
  boost: 0.5
title: CALLERID
---

# CALLERID()

### Synopsis

Gets or sets Caller*ID data on the channel.

### Description

Gets or sets Caller*ID data on the channel. Uses channel callerid by default or optional callerid, if specified.<br>

The _pres_ field gets/sets a combined value for _name-pres_ and _num-pres_.<br>

The allowable values for the _name-charset_ field are the following:<br>


* `unknown` - Unknown<br>

* `iso8859-1` - ISO8859-1<br>

* `withdrawn` - Withdrawn<br>

* `iso8859-2` - ISO8859-2<br>

* `iso8859-3` - ISO8859-3<br>

* `iso8859-4` - ISO8859-4<br>

* `iso8859-5` - ISO8859-5<br>

* `iso8859-7` - ISO8859-7<br>

* `bmp` - ISO10646 Bmp String<br>

* `utf8` - ISO10646 UTF-8 String<br>

### Syntax


```

CALLERID(datatype,CID)
```
##### Arguments


* `datatype` - The allowable datatypes are:<br>

    * `all`

    * `name`

    * `name-valid`

    * `name-charset`

    * `name-pres`

    * `num`

    * `num-valid`

    * `num-plan`

    * `num-pres`

    * `pres`

    * `subaddr`

    * `subaddr-valid`

    * `subaddr-type`

    * `subaddr-odd`

    * `tag`

    * `priv-all`

    * `priv-name`

    * `priv-name-valid`

    * `priv-name-charset`

    * `priv-name-pres`

    * `priv-num`

    * `priv-num-valid`

    * `priv-num-plan`

    * `priv-num-pres`

    * `priv-subaddr`

    * `priv-subaddr-valid`

    * `priv-subaddr-type`

    * `priv-subaddr-odd`

    * `priv-tag`

    * `ANI-all`

    * `ANI-name`

    * `ANI-name-valid`

    * `ANI-name-charset`

    * `ANI-name-pres`

    * `ANI-num`

    * `ANI-num-valid`

    * `ANI-num-plan`

    * `ANI-num-pres`

    * `ANI-tag`

    * `RDNIS`

    * `DNID`

    * `dnid-num-plan`

    * `dnid-subaddr`

    * `dnid-subaddr-valid`

    * `dnid-subaddr-type`

    * `dnid-subaddr-odd`

* `CID` - Optional Caller*ID to parse instead of using the Caller*ID from the channel. This parameter is only optional when reading the Caller*ID.<br>


### Generated Version

This documentation was generated from Asterisk branch 16 using version GIT 