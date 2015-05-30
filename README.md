# Social Vocabulary
Experiment with maintaining a documentation of living vocabulary for Social Web. Not intending to mint new URIs for terms, but instead reuse existing ones and document how one can use them all together by providing illustrated examples!

Inspired by http://lov.okfn.org, http://schema.org, http://microformats.org and http://vocab.org

## Class

### Agent

* Individual
 * Person
* Group
 * Organization
* Daemon
 * Bot
 * Service

### Object

* App (SoftwareApplication)
* Event (social event, distinct from Activity)
* Place
* Tangible
 * Vehicle
 * Device
* Intangible
 * CreativeWork (also Project)

### Activity

* [Follow](activity/Follow)
* Unfollow
* [Subscribe](activity/Subscribe)
* Unsubscribe
* [Join](activity/Join)
* [Leave](activity/Leave)
* [Invite](activity/Invite)
* Accept
* Reject
* [Travel](activity/Travel)
* Arrive (also CheckIn?)
* Depart (also CheckOut?)
* [Transport](activity/Transport)
* Write
* Read
* Edit

### Qualified Relation
* [Containment](qualified-relation/Containment)
* [Following](qualified-relation/Following)
* Subscription
* [Membership](qualified-relation/Membership)
* [Attendance](qualified-relation/Attendance)
* Invitation

### Container

* [DirectContainer](container/DirectContainer)
* Collection
 * MediaGallery
 * AddressBook
 * SubscriptionList
* Stream
* Feed
 * EventCalendar
 * GeoFeed
* Channel
 * MediaChannel
 * MailingList
 * ChatChannel
* Wiki

## Object Property

* [contains](property/contains)
* [follows](property/follows)
* subscribes
* [member](property/member)
* [attendee](property/attendee)
* invitee
* stays
* likes
* achieves

## Data Property

* startTime
* endTime
