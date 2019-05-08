# ![LOGO](logo.png) uebermaps API endpoints **flow**ground Connector

## Description

A generated **flow**ground connector for the uebermaps API endpoints API (version 2.0).

Generated from: https://api.apis.guru/v2/specs/uebermaps.com/2.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:36+03:00

## API Description

Enable people to store spots on public and private maps

## Authorization

This API does not require authorization.

## Actions

### Update account

> Update account. Wrap map parameters in [user].

*Tags:* `Account`

### Delete attachment

> Delete attachment.

*Tags:* `Attachments`

#### Input Parameters
* `id` - _required_ - Attachment id

### Sign in user

> Sign in user. Wrap authentication parameters in [user].

*Tags:* `Authentication`

### List your collaborator invitations

> List your collaborator invitations.

*Tags:* `CollaboratorInvitations`

### Invite user to collaborate on map

> Invite user to collaborate on map.

*Tags:* `CollaboratorInvitations`

### Delete collaborator invitation

> Delete collaborator invitation.

*Tags:* `CollaboratorInvitations`

#### Input Parameters
* `id` - _required_ - Collaborator invitation id

### Show collaborator invitation

*Tags:* `CollaboratorInvitations`

#### Input Parameters
* `id` - _required_ - Collaborator invitation id

### Accept collaborator invitation.

*Tags:* `CollaboratorInvitations`

#### Input Parameters
* `id` - _required_ - Collaborator invitation id

### Delete comment

> Delete comment.

*Tags:* `Comments`

#### Input Parameters
* `id` - _required_ - Comment id

### Update comment

> Update comment. Wrap comment parameters in [comment].

*Tags:* `Comments`

#### Input Parameters
* `id` - _required_ - Comment id

### List your own events

> List your own events.

*Tags:* `Events`

#### Input Parameters
* `timeframe_start` - _optional_ - Begin of time range of event (ISO 8601 date format).
* `timeframe_end` - _optional_ - End of time range of event (ISO 8601 date format).
* `bounds` - _optional_ - To refine your event index request to contain only events within                                                             a geographical box pass the followng bounds parameters.                                                             F. e. to get events within 'Hamburg, St. Pauli':                                                             bounds[sw_lat]=53.54831449741324                                                             bounds[sw_lon]=9.943227767944336                                                             bounds[ne_lat]=53.5571103674878                                                             bounds[ne_lon]=9.9776029586792

### Delete event

> Delete event.

*Tags:* `Events`

#### Input Parameters
* `id` - _required_ - Event id

### Get event

> Get basic information about an event

*Tags:* `Events`

#### Input Parameters
* `id` - _required_ - Id of event

### Update event

> Update event. Wrap event parameters in [event].

*Tags:* `Events`

#### Input Parameters
* `id` - _required_ - Event id

### List your own maps

> List your own maps.

*Tags:* `Maps`

### Create map

> Create map. Wrap map parameters in [map]. To add a map header picture pass a base64 encoded string to [map][picture].

*Tags:* `Maps`

### Search maps

*Tags:* `Search`

#### Input Parameters
* `q` - _optional_ - Query
* `d` - _optional_ - Distance. Diameter of search radius in meter (default: 2000 meter)
* `lat` - _optional_ - Latitude for search radius (default distance: 2000 meter)
* `lon` - _optional_ - Longitude for search radius (default distance: 2000 meter)

### Delete map

> Delete map.

*Tags:* `Maps`

#### Input Parameters
* `id` - _required_ - map id

### Get map

> Get basic information about a map

*Tags:* `Maps`

#### Input Parameters
* `id` - _required_ - Id of map

### Update map

> Update map. Wrap map parameters in [map]. To update the map header picture pass a base64 encoded string to [map][picture].

*Tags:* `Maps`

#### Input Parameters
* `id` - _required_ - map id

### List attachments for a given map

> List attachments for a given map.

*Tags:* `Attachments`

#### Input Parameters
* `id` - _required_ - Map id

### Upload map attachment

> Upload map attachment. Wrap attachment parameters in [attachment]

*Tags:* `Attachments`

#### Input Parameters
* `id` - _required_ - Map id

### List collaborators of a map

> List collaborators of a map.

*Tags:* `Collaborators`

#### Input Parameters
* `id` - _required_ - Map id

### Delete collaboration

> Delete collaboration.

*Tags:* `Collaborators`

#### Input Parameters
* `id` - _required_ - map id
* `user_id` - _required_ - user id

### Update collaborator

> Update collaborator. Wrap collaborator parameters in [collaborator]

*Tags:* `Collaborators`

#### Input Parameters
* `id` - _required_ - map id
* `user_id` - _required_ - user id

### List comments for a given map

> List comments for a given map.

*Tags:* `Comments`

#### Input Parameters
* `id` - _required_ - Id of map

### Create map comment

> Create map comment. Wrap comment parameters in [comment].

*Tags:* `Comments`

#### Input Parameters
* `id` - _required_ - map id

### List respots of a map

> List respots of a map.

*Tags:* `Respots`

#### Input Parameters
* `id` - _required_ - Map Id

### List spots for a given map

> List spots for a given map.

*Tags:* `Spots`

#### Input Parameters
* `id` - _required_ - Id of map
* `order` - _optional_ - Order of spots
    Possible values: created_at_asc, created_at_desc, updated_at_asc, updated_at_desc, title_asc, title_desc.

### Create spot

> Create spot. Wrap parameters in [spot]. To add a spot picture pass a base64 encoded string to [spot][picture].

*Tags:* `Spots`

#### Input Parameters
* `id` - _required_ - Id of map

### Unsubscribe from map

> Unsubscribe from map.

*Tags:* `Subscriptions`

#### Input Parameters
* `id` - _required_ - map id

### List subscriptions for a given map

> List subscriptions for a given map.

*Tags:* `Subscriptions`

#### Input Parameters
* `id` - _required_ - Id of map

### Get spot

> Get basic information about a spot

*Tags:* `Spots`

#### Input Parameters
* `id` - _required_ - Id of spot
* `map_id` - _required_ - Id of map

### Delete respot from map by spot id

> Delete respot from map by spot id.

*Tags:* `Respots`

#### Input Parameters
* `map_id` - _required_ - Map Id
* `spot_id` - _required_ - Spot Id

### List maps that user can respot to

> List maps that user can respot to.

*Tags:* `Respots`

### Delete respot

> Delete respot.

*Tags:* `Respots`

#### Input Parameters
* `id` - _required_ - Respot Id

### Get respot

> Get basic information about a respot

*Tags:* `Respots`

#### Input Parameters
* `id` - _required_ - Id of respot

### Get secret access token to share map

> Get secret access token of an uebermap with access set to 'Secret link'. Pass the 'token' on every request you make to access this uebermap and its resources. F.e. token=1-x_gqu7eLBe3uKoAGAGXy

*Tags:* `Share`

#### Input Parameters
* `id` - _required_ - Id of map

### List your own spots

> List your own spots.

*Tags:* `Spots`

#### Input Parameters
* `order` - _optional_ - Order of spots
    Possible values: created_at_asc, created_at_desc, updated_at_asc, updated_at_desc, title_asc, title_desc.

### Search spots

*Tags:* `Search`

#### Input Parameters
* `q` - _optional_ - Query
* `d` - _optional_ - Distance. Diameter of search radius in meter (default: 2000 meter)
* `lat` - _optional_ - Latitude for search radius (2 km)
* `lon` - _optional_ - Longitude for search radius (2 km)

### Delete spot

> Delete spot.

*Tags:* `Spots`

#### Input Parameters
* `id` - _required_ - spot id

### Update spot

> Update spot. Wrap parameters in [spot]. To update the spot picture pass a base64 encoded string to [spot][picture].

*Tags:* `Spots`

#### Input Parameters
* `id` - _required_ - spot id

### List attachments for a given spot

> List attachments for a given spot.

*Tags:* `Attachments`

#### Input Parameters
* `id` - _required_ - Spot id

### Upload spot attachment

> Upload spot attachment. Wrap attachment parameters in [attachment]

*Tags:* `Attachments`

#### Input Parameters
* `id` - _required_ - Spot id

### List comments for a given spot

> List comments for a given spot.

*Tags:* `Comments`

#### Input Parameters
* `id` - _required_ - Id of spot

### Create spot comment

> Create spot comment. Wrap comment parameters in [comment].

*Tags:* `Comments`

#### Input Parameters
* `id` - _required_ - spot id

### List events for a given spot

> List maps for a given spot.

*Tags:* `Events`

#### Input Parameters
* `id` - _required_ - Id of spot
* `timeframe_start` - _optional_ - Begin of time range of event (ISO 8601 date format).
* `timeframe_end` - _optional_ - End of time range of event (ISO 8601 date format).
* `bounds` - _optional_ - To refine your event index request to contain only events within                                                             a geographical box pass the followng bounds parameters.                                                             F. e. to get events within 'Hamburg, St. Pauli':                                                             bounds[sw_lat]=53.54831449741324                                                             bounds[sw_lon]=9.943227767944336                                                             bounds[ne_lat]=53.5571103674878                                                             bounds[ne_lon]=9.9776029586792

### Create event

> Create event. Wrap map parameters in [event].

*Tags:* `Events`

#### Input Parameters
* `id` - _required_ - Spot id

### Respot a spot onto a map

> Respot a spot onto a map.

*Tags:* `Respots`

#### Input Parameters
* `id` - _required_ - Spot Id

### List subscriptions. Pass no parameters to get own subscriptions

> List subscriptions.

*Tags:* `Subscriptions`

#### Input Parameters
* `user_id` - _optional_ - Id of user
* `map_id` - _optional_ - Id of map

### Create map subscription

> Create map subscription.

*Tags:* `Subscriptions`

### List latest maps

> List latest maps.

*Tags:* `Trends`

### List recommended maps

> List recommended maps.

*Tags:* `Trends`

### Search users

*Tags:* `Search`

#### Input Parameters
* `q` - _optional_ - Query

### Get user profile

> Get profile a user

*Tags:* `Users`

#### Input Parameters
* `id` - _required_ - Id of user

### List maps for a given user

> List maps for a given user.

*Tags:* `Maps`

#### Input Parameters
* `user_id` - _required_ - Id of user

## License

**flow**ground :- Telekom iPaaS / uebermaps-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
