# Membership
(qualified relation)

Relationship where a group has a member.

* property: **[member](../../property/member)**
* subject: **[Group](../../agent/Group)**
* object: **[Person](../../agent/Person)**
* activity: **[Join](../../activity/Join)**,
  **[Leave](../../activity/Leave)**

## Examples

### Group with a member
*elf Pavlik member of Social WG*

![Membership](https://docs.google.com/drawings/d/1BG6yMItozgB3ocLgqVXbaMWGfRYoZ9GmZddWgKNwIqA/pub?w=1016&h=556)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" ;
  :member <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/3242> a :Membership ;
  rdf:subject <http://www.w3.org/Social/WG> ;
  rdf:predicate :member ;
  rdf:object <https://wwelves.org/perpetual-tripper> ;
  :startTime "10 Sep 2014" .
```

