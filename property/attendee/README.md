# attendee
(property)

A group with people as its members

* recommended inverse name: **attendeeIn**
* subject: **[Event](../../object/Event)**
* object: **[Individual](../../agent/Individual)**
* qualified relation: **[Attendance](../../qualified-relation/Attendance)**
* activity: **[Join](../../activity/Join)**, **[Leave](../../activity/Leave)**, Arrive, Depart


## Examples

### Event with an attendee
*elf Pavlik attendee in Social WG: F2F3*

![attendee](https://docs.google.com/drawings/d/1mcajh_yRy03B5J-Vkuqs8rlTWb_MA97XBr-t1YeTBHQ/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<https://www.w3.org/wiki/Socialwg/2015-05-04> a :Event ;
  :name "Social WG: F2F3" ;
  :member <https://wwelves.org/perpetual-tripper> .
```
