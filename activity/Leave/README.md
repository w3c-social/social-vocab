# Leave
(activity)

Act of an agent joining a group or an event

* activity: **[Join](../Join)**
* property: **[member](../../property/member)**, **[attendee](../../property/attendee)**
* qualified relation: **[Membership](../../qualified-relation/Membership)**, **[Attendance](../../qualified-relation/Attendance)**
* agent & object: Person, Group, Event

## Examples

### Person leaves Group
*elf Pavlik leaves Social WG* 

![Leave](https://docs.google.com/drawings/d/18wELALmdwlkU4apLebPoMNEGrIHyZTc3cQk6AbFSalM/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" ;
  # this relation will get removed
  :member <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/19012> a :Membership
  rdf:subject <http://www.w3.org/Social/WG> ;
  rdf:object <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :member ;
  :startTime "12 Sep 2014" .
  :endTime "6 Dec 2016" .

<https://wwelves.org/perpetual-tripper/log/20153> a :Leave ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:object <http://www.w3.org/Social/WG> ;
  as:result <https://wwelves.org/perpetual-tripper/rel/19012> .
```

### Person leaves Event
*elf Pavlik leaves Social WG: F2F3* 

![Leave](https://docs.google.com/drawings/d/1QOZI18VoMvjJRGbsxN3ech5P0olJVNvGSIvkn9Op1io/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<https://www.w3.org/wiki/Socialwg/2015-05-04> a :Event
  :name "Social WG: F2F3" ;
  # this relation will get removed
  :attendee <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/19012> a :Attendance
  rdf:subject <https://www.w3.org/wiki/Socialwg/2015-05-04> ;
  rdf:object <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :member ;
  :startTime "18 Mar 2015" .
  :endTime "29 Apr 2015" .

<https://wwelves.org/perpetual-tripper/log/20153> a :Leave ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:object <https://www.w3.org/wiki/Socialwg/2015-05-04> ;
  as:result <https://wwelves.org/perpetual-tripper/rel/19012> .
```
