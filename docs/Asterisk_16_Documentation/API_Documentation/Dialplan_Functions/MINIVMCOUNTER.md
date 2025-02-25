---
search:
  boost: 0.5
title: MINIVMCOUNTER
---

# MINIVMCOUNTER()

### Synopsis

Reads or sets counters for MiniVoicemail message.

### Description

The operation is atomic and the counter is locked while changing the value. The counters are stored as text files in the minivm account directories. It might be better to use realtime functions if you are using a database to operate your Asterisk.<br>


### Syntax


```

MINIVMCOUNTER(account:name:operand)
```
##### Arguments


* `account` - If account is given and it exists, the counter is specific for the account.<br>
If account is a domain and the domain directory exists, counters are specific for a domain.<br>

* `name` - The name of the counter is a string, up to 10 characters.<br>

* `operand` - The counters never goes below zero. Valid operands for changing the value of a counter when assigning a value are:<br>

    * `i` - Increment by value.<br>

    * `d` - Decrement by value.<br>

    * `s` - Set to value.<br>

### See Also

* [Dialplan Applications MinivmRecord](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/MinivmRecord)
* [Dialplan Applications MinivmGreet](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/MinivmGreet)
* [Dialplan Applications MinivmNotify](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/MinivmNotify)
* [Dialplan Applications MinivmDelete](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/MinivmDelete)
* [Dialplan Applications MinivmAccMess](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/MinivmAccMess)
* [Dialplan Applications MinivmMWI](/Asterisk_16_Documentation/API_Documentation/Dialplan_Applications/MinivmMWI)
* [Dialplan Functions MINIVMACCOUNT](/Asterisk_16_Documentation/API_Documentation/Dialplan_Functions/MINIVMACCOUNT)


### Generated Version

This documentation was generated from Asterisk branch 16 using version GIT 