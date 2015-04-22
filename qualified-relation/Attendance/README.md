# Attendance
(qualified relation)

Relationship where an event has an attendee.

* property: **[attendee](../../property/attendee)**
* subject: **[Event](../../agent/Event)**
* object: **[Person](../../agent/Person)**
* activity: **[Join](../../activity/Join)**,
  **[Leave](../../activity/Leave)**, Arrive, Depart

## Examples

### Event with an attendee
*elf Pavlik attendee in Social WG*

![Attendance](https://docs.google.com/drawings/d/1WQaXja2Q6cu_jVLf60umYdbbY1XBjBpJWUIdgSbNHUU/pub?w=1016&h=556)

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
```

