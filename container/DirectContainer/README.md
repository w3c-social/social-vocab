# DirectContainer
(container)

Container allowing defining particular relationship between certain resource and
all the contained elements.

* property: **[contains](../../property/contains)**
* qualified relation:
  **[Containment](../../qualified-relation/Containment)**

## Examples

### Followers of a group
*elf Pavlik and Amy Guy follow Social WG*

![DirectContainer](https://docs.google.com/drawings/d/10erXDrL-im1mXta8STad4BAsZYzbbPQhcqr8Ld2trWU/pub?w=896&h=489)

```ttl
<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" ;

<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik" ;

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" .

<http://www.w3.org/Social/WG/followed-by> a ldp:DirectContainer ;
  ldp:membershipResource <http://www.w3.org/Social/WG/followed-by> ;
  ldp:isMemberOfRelation :follows ;
  ldp:contains <https://wwelves.org/perpetual-tripper> ,
    <https:/rhiaro.co.uk> .
```

### Person following agents
*elf Pavlik follows Amy Guy and Social WG*

![DirectContainer](https://docs.google.com/drawings/d/1wq0_hOYRopXmdEAzcxz9E5NF0XVXNZuUfPS6tI7VkG8/pub?w=896&h=489)

```ttl
<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" .

<http://www.w3.org/Social/WG> a :Group ;
  :name "Social WG" .

<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik" ;

<https://wwelves.org/perpetual-tripper/follows> a ldp:DirectContainer ;
  ldp:membershipResource <http://www.w3.org/Social/WG/followed-by> ;
  ldp:hasMemberRelation :follows ;
  ldp:contains <https:/rhiaro.co.uk> ,
    <http://www.w3.org/Social/WG> .

```
