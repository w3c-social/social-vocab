# Following
(qualified relation)

Relationship where one agent follows another agent.

* verb: **[follows](../../verb/follows)**
* activity: **[Follow](../../activity/Follow)**

![Following](https://docs.google.com/drawings/d/1K0KRBQEdIm3eMLh1YZKgw44m5516lpvKcqSkTcJPIls/pub?w=960&h=540)

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
```

