# member
(property)

A group with individuals as its members

* recommended inverse name: **memberOf**
* subject: **[Group](../../agent/Group)**
* object: **[Individual](../../agent/Individual)**
* qualified relation: **[Membership](../../qualified-relation/Membership)**
* activity: **[Join](../../activity/Join)**, **[Leave](../../activity/Leave)**

## Examples

### Group with a member
*elf Pavlik member of Social WG*

![member](https://docs.google.com/drawings/d/1tzPRzpnuyjH8QoVcqjRngEEwKoIOpMgFwQOLXq3bRVE/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* .

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" ;
  :member <https://wwelves.org/perpetual-tripper> .
```
