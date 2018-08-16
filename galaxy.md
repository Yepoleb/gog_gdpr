# Galaxy

All dates are in the strftime format "%Y-%m-%d %H-%M-%S".

## achievements

* `client_id`: User ID
* `name`: Achievement name
* `description`: Achievement description
* `date_unlocked`: Date unlocked
* `unlocked`: Is unlocked
* `date_revealed`: Date the achievement has become visible to the user (probably used for hidden achievements)
* `revealed`: Is revealed
* `progress`: Unknown

## chatConversations

Note: This file is not included in the dump because it containes personal data of other people.

* `room_id`: 64 bit Room ID
* `username`: User writing the message
* `content`: Message text
* `message_state`: Unknown
* `date_created`: Date message was sent
* `date_updated`: Date message was updated, never significantly differs from created
* `type`: Unknown
* `room_name`: Conversation partner
* `date_last_active`: Date of last activity in the room
* `unread_message_count`: Unread messages in the room
* `room_state`: Unknown

## friends

* `user_id`: Own user ID
* `friend_user_id`: Friend's user ID
* `date_created`: Date friend invite was sent
* `date_accepted`: Date friend invide was accepted

## gameTimeSessions

* `game_id`: Product ID
* `time`: Time spent in game
* `date_created`: Date the game was launched

## gameTimeSummary

* `game_id`: Product ID
* `time`: Total time spent in game
* `sessions_count`: Times the game has been launched
* `date_created`: Date game was first launched
* `date_updated`: Date game was last launched

## profile

* `username`: Profile name
* `email`: Email address
* `date_created`: Date the account was created
* `avatar`: URL to avatar
* `settings.allow_to_be_invited_by`: Who can invite you. Known values: `anyone`
* `settings.allow_to_be_seached`: Account can be searched for
* `settings.use_two_step_authentication`: Account uses two step login

## proposedFriends

Note: This file is not included in the dump because it containes personal data of other people.

* `proposed_to_user_id`: Own user ID
* `source`: Recommendation source (probably to differenciate Facebook recommendations). Known values: `internal`
* `proposed_user_id`: Recommended friend ID
* `meta.common_friends`: Friends in common with id, name and avatar
* `date_created`: Date the suggestion was generated

