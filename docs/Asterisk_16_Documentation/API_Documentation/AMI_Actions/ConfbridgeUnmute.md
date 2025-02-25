---
search:
  boost: 0.5
title: ConfbridgeUnmute
---

# ConfbridgeUnmute

### Synopsis

Unmute a Confbridge user.

### Description


### Syntax


```


    Action: ConfbridgeUnmute
    ActionID: <value>
    Conference: <value>
    Channel: <value>

```
##### Arguments


* `ActionID` - ActionID for this transaction. Will be returned.<br>

* `Conference`

* `Channel` - If this parameter is not a complete channel name, the first channel with this prefix will be used.<br>
If this parameter is "all", all channels will be unmuted.<br>
If this parameter is "participants", all non-admin channels will be unmuted.<br>


### Generated Version

This documentation was generated from Asterisk branch 16 using version GIT 