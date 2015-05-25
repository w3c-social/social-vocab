# Invite
(activity)

Act of an agent joining a group or an event

* activity: **Accept**, **Reject**
* property: **[invitee]**
* qualified relation: **Invitation**
* agent & object: Person, Group, Event

## Examples

### Person invites Person to Group
*elf Pavlik joins Social WG* 

![Invite]()

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" .

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" ;
  :member <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/19012> a :Invitation
  rdf:subject <http://www.w3.org/Social/WG> ;
  rdf:object <https://rhiaro.co.uk> ;
  dc:author  <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :invitee ;
  :startTime "12 Sep 2014" .

<https://wwelves.org/perpetual-tripper/log/20153> a :Invite ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:object <https://rhiaro.co.uk> ;
  as:target <http://www.w3.org/Social/WG> ;
  as:result <https://wwelves.org/perpetual-tripper/rel/19012> .
```

### Person invites Person to Event
*elf Pavlik joins Social WG: F2F3* 

![Invite]()

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" .

<https://www.w3.org/wiki/Socialwg/2015-05-04> a :Event
  :name "Social WG: F2F3" ;
  :attendee <https://wwelves.org/perpetual-tripper> .

<https://wwelves.org/perpetual-tripper/rel/19012> a :Invitation
  rdf:subject <https://www.w3.org/wiki/Socialwg/2015-05-04> ;
  rdf:object <https://rhiaro.co.uk> ;
  dc:author  <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :invitee ;
  :startTime "12 Sep 2014" .

<https://wwelves.org/perpetual-tripper/log/20153> a :Invite ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:object <https://rhiaro.co.uk> ;
  as:target <https://www.w3.org/wiki/Socialwg/2015-05-04> ;
  as:result <https://wwelves.org/perpetual-tripper/rel/19012> .
```
