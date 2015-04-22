# Join
(activity)

Act of an agent joining a group or an event

* activity: **[Invite](../../activity/Invite)**, **[Leave](../Leave)**
* property: **[member](../../property/member)**, **[attendee](../../property/attendee)**
* qualified relation: **[Membership](../../qualified-relation/Membership)**, **[Attendance](../../qualified-relation/Attendance)**
* agent & object: Person, Group, Event

## Examples

### Person joins Group
*elf Pavlik joins Social WG* 

![Join](https://docs.google.com/drawings/d/1UGHmz8olXL3zKmYWYqC9h231vUiwE8LfG8xoeg8ofsU/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" ;
  :member <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/19012> a :Membership
  rdf:subject <http://www.w3.org/Social/WG> ;
  rdf:object <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :member ;
  :startTime "12 Sep 2014" .

<https://wwelves.org/perpetual-tripper/log/20153> a :Join ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:object <http://www.w3.org/Social/WG> ;
  as:result <https://wwelves.org/perpetual-tripper/rel/19012> .
```

### Person joins Event
*elf Pavlik joins Social WG: F2F3* 

![Join](https://docs.google.com/drawings/d/1FobXsV0-xyWU8pC9Ad7M_LrDt4TKzKcCVWdPpE1OTgY/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<https://www.w3.org/wiki/Socialwg/2015-05-04> a :Event
  :name "Social WG: F2F3" ;
  :attendee <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/19012> a :Attendance
  rdf:subject <https://www.w3.org/wiki/Socialwg/2015-05-04> ;
  rdf:object <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :member ;
  :startTime "18 Mar 2015" .

<https://wwelves.org/perpetual-tripper/log/20153> a :Join ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:object <https://www.w3.org/wiki/Socialwg/2015-05-04> ;
  as:result <https://wwelves.org/perpetual-tripper/rel/19012> .
```
