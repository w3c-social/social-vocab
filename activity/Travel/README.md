# Travel
(verb)

Act of traveling from origin to destination.

see also: Stay

* relation: **[present](../../relation/present)** (agent at origin and destination)

same value for as:actor and as:object
union of Depart and Arrive
as:result Traveling and possibly Arriving and Departing

![follows](https://docs.google.com/drawings/d/1KS7T38IAFj6CG77_CcJbGsgwEm0ndngCeOTXGIT1JO8/pub?w=1138&h=780)

```ttl
# Agents & Objects
<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik" .

<http://sws.geonames.org/2950159/> a :City ;
  :name "Berlin" .

<http://sws.geonames.org/2988507/> a :City ;
  :name "Paris" .

<https://plp.hackers4peace.net/30492840928420348293> a :Bus .


# Activities
<https://wwelves.org/perpetual-tripper/log/393932432> a :Depart ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:origin <http://sws.geonames.org/2950159/> ;
  as:instrument <https://plp.hackers4peace.net/30492840928420348293> ;
  :startTime "30 April 2015" .

<https://wwelves.org/perpetual-tripper/log/3939391010> a :Arrive ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:destination <http://sws.geonames.org/29507/> ;
  as:instrument <https://plp.hackers4peace.net/30492840928420348293> ;
  :endTime "30 April 2015" .

<https://wwelves.org/perpetual-tripper/log/3939392> a :Travel ;
  as:actor <https://wwelves.org/perpetual-tripper> ;
  as:origin <http://sws.geonames.org/2950159/> ;
  as:destination <http://sws.geonames.org/29507/> ;
  as:instrument <https://plp.hackers4peace.net/30492840928420348293> ;
  :startTime "30 April 2015" ;
  :endTime "30 April 2015" ;
  :contains <https://wwelves.org/perpetual-tripper/log/393932432> ,
    <https://wwelves.org/perpetual-tripper/log/3939391010> .

# Qualified Relations
<https://wwelves.org/perpetual-tripper/rel/393013> a :Presence ;
  rdf:subject <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :present ;
  rdf:object <http://sws.geonames.org/2988159/> ;
  :interaction <https://wwelves.org/perpetual-tripper/log/393932432> .

<https://wwelves.org/perpetual-tripper/rel/393210> a :Presence ;
  rdf:subject <https://wwelves.org/perpetual-tripper> ;
  rdf:predicate :present ;
  rdf:object <http://sws.geonames.org/2988507/> ;
  :interaction <https://wwelves.org/perpetual-tripper/log/3939391010> .
```
