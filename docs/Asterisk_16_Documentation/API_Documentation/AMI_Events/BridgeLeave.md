---
search:
  boost: 0.5
title: BridgeLeave
---

# BridgeLeave

### Synopsis

Raised when a channel leaves a bridge.

### Syntax


```


    Event: BridgeLeave
    BridgeUniqueid: <value>
    BridgeType: <value>
    BridgeTechnology: <value>
    BridgeCreator: <value>
    BridgeName: <value>
    BridgeNumChannels: <value>
    BridgeVideoSourceMode: <value>
    [BridgeVideoSource:] <value>
    Channel: <value>
    ChannelState: <value>
    ChannelStateDesc: <value>
    CallerIDNum: <value>
    CallerIDName: <value>
    ConnectedLineNum: <value>
    ConnectedLineName: <value>
    Language: <value>
    AccountCode: <value>
    Context: <value>
    Exten: <value>
    Priority: <value>
    Uniqueid: <value>
    Linkedid: <value>

```
##### Arguments


* `BridgeUniqueid`

* `BridgeType` - The type of bridge<br>

* `BridgeTechnology` - Technology in use by the bridge<br>

* `BridgeCreator` - Entity that created the bridge if applicable<br>

* `BridgeName` - Name used to refer to the bridge by its BridgeCreator if applicable<br>

* `BridgeNumChannels` - Number of channels in the bridge<br>

* `BridgeVideoSourceMode` - 
    * `none`

    * `talker`

    * `single`
The video source mode for the bridge.<br>

* `BridgeVideoSource` - If there is a video source for the bridge, the unique ID of the channel that is the video source.<br>

* `Channel`

* `ChannelState` - A numeric code for the channel's current state, related to ChannelStateDesc<br>

* `ChannelStateDesc`

    * `Down`

    * `Rsrvd`

    * `OffHook`

    * `Dialing`

    * `Ring`

    * `Ringing`

    * `Up`

    * `Busy`

    * `Dialing Offhook`

    * `Pre-ring`

    * `Unknown`

* `CallerIDNum`

* `CallerIDName`

* `ConnectedLineNum`

* `ConnectedLineName`

* `Language`

* `AccountCode`

* `Context`

* `Exten`

* `Priority`

* `Uniqueid`

* `Linkedid` - Uniqueid of the oldest channel associated with this channel.<br>

### Class

CALL
### See Also

* [AMI Events BridgeCreate](/Asterisk_16_Documentation/API_Documentation/AMI_Events/BridgeCreate)
* [AMI Events BridgeDestroy](/Asterisk_16_Documentation/API_Documentation/AMI_Events/BridgeDestroy)
* [AMI Events BridgeEnter](/Asterisk_16_Documentation/API_Documentation/AMI_Events/BridgeEnter)


### Generated Version

This documentation was generated from Asterisk branch 16 using version GIT 