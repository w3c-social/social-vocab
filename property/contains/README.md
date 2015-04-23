# contains
(property)

Container containing resources.

* recommended inverse name: **containedBy**
* subject: Container
* qualified relation:
  **[Containment](../../qualified-relation/Containment)**
* activity: **[Add](../../activity/Add)**,
  **[Remove](../../activity/Remove)**,
  **[Move](../../activity/Move)**

## Examples

### Container contains Person
*List of Social WG followers contains elf Pavlik*

![contains](https://docs.google.com/drawings/d/1yhQ-OJu51XWQxsR-HDf9usaIYugnbKiDvqWlaXQ7joM/pub?w=960&h=540)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* ;

<http://www.w3.org/Social/WG/followed-by> a ldp:DirectContainer ;
  :name "List of Social WG followers* ;
  ldp:contains <https://wwelves.org/perpetual-tripper> .
```
