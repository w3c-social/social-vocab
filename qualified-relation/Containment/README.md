# Containment
(qualified relation)

Relationship where container contains a resource.

* property: **[contains](../../property/contains)**
* subject: **[Container](../../agent/Container)**
* object: **[Thing](../../object/Thing)**

## Examples

### Container contains Person
*List of Social WG followers contains elf Pavlik*

![Containment](https://docs.google.com/drawings/d/1TXnPIR1_etvsSzqgGnqdflChkmiOpqMIOTReG9SVODo/pub?w=939&h=547)

```ttl
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik" ;

<http://www.w3.org/Social/WG/followed-by> a ldp:DirectContainer ;
  ldp:contains <https://wwelves.org/perpetual-tripper>  .


<http://www.w3.org/Social/WG/rel/3242> a :Containment ;
  rdf:subject <http://www.w3.org/Social/WG/followed-by> ;
  rdf:predicate :contains ;
  rdf:object <https://wwelves.org/perpetual-tripper> ;
  owl:sameAs <https://wwelves.org/perpetual-tripper/rel/3902> ;
  :startTime "20 Aug 2014" .

```
