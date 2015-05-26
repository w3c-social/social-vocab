# Subscribe
(activity)

Act of subscribing to a channel

* property: **subscribes**
* qualified relation: **Subscription**

![Subscribe](https://docs.google.com/drawings/d/1cFUapuMTxDt7JsjwgfqmwsE88mez8V4aL8jcR4QPJPQ/pub?w=1234&h=747)

```ttl
<https:/rhiaro.co.uk> a :Person ;
  :name "Amy Guy" ;
  :outbox <https:/rhiaro.co.uk/log> ;
  :stream <https:/rhiaro.co.uk/sport> ;
  :feed <https:/rhiaro.co.uk/bookmarks> ,
    <https:/rhiaro.co.uk/notes> ;
  :map <https:/rhiaro.co.uk/map> ;
  :calendar <https:/rhiaro.co.uk/calendar> .

<https:/rhiaro.co.uk/log> a as:Collection ;
  :name "all the Amy's activities" .

<https:/rhiaro.co.uk/sport> a as:Collection ;
  :name "Amy's sport activities" .

<https:/rhiaro.co.uk/bookmarks> a sioc:BookmarkFolder ;
  :name "Amy's bookmarks" .

<https:/rhiaro.co.uk/notes> a h:Feed ;
  :name "Amy's notes" .

<https:/rhiaro.co.uk/map> a :GeoFeed ;
  :name "Amy's map" .

<https:/rhiaro.co.uk/calendar> a sioc:EventCalendar ;
  :name "Amy's calendar" .

<https://wwelves.org/perpetual-tripper> a :Person ;
  :name "elf Pavlik" ;
  :follows <https://rhiaro.co.uk> .

<https://wwelves.org/perpetual-tripper/log/2762> a :Follow ;
  as:actor `<https://wwelves.org/perpetual-tripper> ;
  as:object <https:/rhiaro.co.uk> ;
  as:result `<https://wwelves.org/perpetual-tripper/rel/3242> .

<https://wwelves.org/perpetual-tripper/log/2762> a :Subscribe ;
  as:actor `<https://wwelves.org/perpetual-tripper> ;
  as:object <https:/rhiaro.co.uk/log> ;
  as:result `<https://wwelves.org/perpetual-tripper/rel/32132> .
```
