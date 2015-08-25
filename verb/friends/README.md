# friends
verb (object property)

An agent friending another agent

* subject: **[Agent](../../agent/Agent)**
* object: **[Agent](../../agent/Agent)**
* qualified relation: **Friending**
* activity: **Friend**
* undo: yes

## Examples

### Two people friend each other
*elf Pavlik and Justine Testing friend each other*

![likes](https://docs.google.com/drawings/d/19ec81cfmoDwGjnQSADEduO7PpdacO0Y8k2YGgepyW_c/pub?w=1161&h=584)

```json
{
  "@context": [
    "http://www.w3.org/ns/activitystreams",
    "https://w3id.org/social/v1"
  ],
  "@graph": [
    {
      "@id": "https://wwelves.org/perpeual-tripper",
      "@type": "Person",
      "displayName": "elf Pavlik",
      "friends": [
        "https://hackers4peace.net/just-testing"
      ],
      "relation": [
        "https://graph.wwelves.org/a497cc30-02eb-4194-8235-c7e58918449f"
      ]
    },
    {
      "@id": "https://hackers4peace.net/just-testing",
      "@type": "Bot",
      "displayName": "Justine Testing",
      "friends": [
        "https://wwelves.org/perpeual-tripper"
      ],
      "relation": [
        "https://graph.hackers4peace.net/f2420dc4-e37a-49be-9305-621303e69885"
      ]
    },
    {
      "@id": "https://graph.wwelves.org/a497cc30-02eb-4194-8235-c7e58918449f",
      "@type": "Relation",
      "subject": "https://wwelves.org/perpeual-tripper",
      "object": "https://hackers4peace.net/just-testing",
      "property": "friends",
      "createdAt": "2015-02-10T15:04:55Z",
      "mirror": "https://graph.hackers4peace.net/f2420dc4-e37a-49be-9305-621303e69885"
    },
    {
      "@id": "https://graph.hackers4peace.net/f2420dc4-e37a-49be-9305-621303e69885",
      "@type": "Relation",
      "subject": "https://hackers4peace.net/just-testing",
      "object": "https://wwelves.org/perpeual-tripper",
      "property": "friends",
      "createdAt": "2015-02-10T15:04:57Z",
      "mirror": "https://graph.wwelves.org/a497cc30-02eb-4194-8235-c7e58918449f"
    }
  ]
}
```
