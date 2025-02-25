---
search:
  boost: 0.5
title: Playback
---

# Playback()

### Synopsis

Play a file.

### Description

Plays back given filenames (do not put extension of wav/alaw etc). The Playback application answers the channel if no options are specified. If the file is non-existent it will fail.<br>

This application sets the following channel variable upon completion:<br>


* `PLAYBACKSTATUS` - The status of the playback attempt as a text string.<br>

    * `SUCCESS`

    * `FAILED`
See Also: Background (application) -- for playing sound files that are interruptible<br>

WaitExten (application) -- wait for digits from caller, optionally play music on hold<br>


### Syntax


```

Playback(filename&[filename2[&...]],[options])
```
##### Arguments


* `filenames`

    * `filename` **required**

    * `filename2[,filename2...]`

* `options` - Comma separated list of options<br>

    * `skip` - Do not play if not answered<br>


    * `noanswer` - Playback without answering, otherwise the channel will be answered before the sound is played.<br>


    * `say` - Play using the say.conf file.<br>


    * `mix` - Play using a mix of filename and the say.conf file.<br>


### See Also

* [Dialplan Applications Background](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/Background)
* [Dialplan Applications WaitExten](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/WaitExten)
* [Dialplan Applications ControlPlayback](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/ControlPlayback)
* [AGI Commands stream_file](/Asterisk_16_Documentation/API_Documentation/AGI_Commands/stream_file)
* [AGI Commands control_stream_file](/Asterisk_16_Documentation/API_Documentation/AGI_Commands/control_stream_file)
* [AMI Actions ControlPlayback](/Asterisk_16_Documentation/API_Documentation/AMI_Actions/ControlPlayback)


### Generated Version

This documentation was generated from Asterisk branch 16 using version GIT 