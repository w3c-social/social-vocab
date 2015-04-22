# follows
(property)

An agent following another agent

* recommended inverse name: **followedBy**
* subject: **[Agent](../../agent/Agent)**
* object: **[Agent](../../agent/Agent)**
* qualified relation: **[Following](../../qualified-relation/Following)**
* activity: **[Follow](../../activity/Follow)**,
  **[Unfollow](../../activity/Unfollow)**

## Examples

### Person follows Person
*elf Pavlik follows Amy Guy*

![follows](https://docs.google.com/drawings/d/1ew_U7Emc8qyQuRRcfzUhab2lmgkv2VHk8JYZYBYgx9E/pub?w=960&h=540)

```ttl
<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" .

<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* ;
  :follows <https://rhiaro.co.uk> .
```
