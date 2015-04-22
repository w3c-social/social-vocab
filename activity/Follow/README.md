# Follow
(activity)

Act of following another agent

* property: **[follows](../../verb/follows)**
* qualified relation: **[Following](../../qualified-relation/Following)**

![follows](https://docs.google.com/drawings/d/1zFWdjo_phs60Lr7dyoXyd4PQ9hOBxadlU8FZDQIAPHg/pub?w=960&h=540)

```ttl
<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" .

<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik* ;
  :follows <https://rhiaro.co.uk> .

<https://wwelves.org/perpetual-tripper/rel/3242> a :Following ;
  rdf:subject <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :follows ;
  rdf:object <https:/rhiaro.co.uk> ;
  :startTime "16 July 2014" .

<https://wwelves.org/perpetual-tripper/log/2762> a :Follow ;
  as:actor `<https://wwelves.org/perpetual-tripper> ;
  as:object <https:/rhiaro.co.uk> ;
  as:result `<https://wwelves.org/perpetual-tripper/rel/3242> .
```
