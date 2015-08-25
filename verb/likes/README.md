# likes
verb (object property)

An agent liking another thing

* recommended inverse name: **likedBy**
* subject: **[Agent](../../agent/Agent)**
* object: **Thing**
* qualified relation: **Liking**
* activity: **Like**, **Dislike**
* undo: yes

## Examples

### Person likes Video
*elf Pavlik likes 'Squaredancing in Berlin' video*

![likes](https://docs.google.com/drawings/d/16uPuEOZi0azfmw6CINwxSkFvddoHSJR5pOCMqpB2xsw/pub?w=1048&h=538)

```json
{
  "@context": [
    "http://www.w3.org/ns/activitystreams",
    "https://w3id.org/social/v1"
  ],
  "@graph": [
    {
      "@id": "https://etv.example/squaredance",
      "@type": "Video",
      "displayName": "Squaredancing in Berlin",
      "@reverse": {
        "likes": [
          "https://wwelves.org/perpetual-tripper"
        ]
      }
    },
    {
      "@id": "https://wwelves.org/perpeual-tripper",
      "@type": "Person",
      "displayName": "elf Pavlik",
      "likes": [
        "https://etv.example/squaredance"
      ],
      "relation": [
        "https://graph.wwelves.org/157e5753-5760-4103-9f5c-742577847e7f"
      ]
    },
    {
      "@id": "https://graph.wwelves.org/157e5753-5760-4103-9f5c-742577847e7f",
      "@type": "Relation",
      "subject": "https://wwelves.org/perpeual-tripper",
      "object": "https://etv.example/squaredance",
      "property": "likes",
      "createdAt": "2015-02-10T15:04:55Z"
    }
  ]
}
```
