# Changelog
All notable changes to this project will be documented in this file.

## 3.2.4 – 2018-07-12
### Added
- Allow external signaling servers to integrate a MCU
  [#398](https://github.com/nextcloud/spreed/pull/398)

### Fixed
- Support chat with a standalone signaling servers
  [#890](https://github.com/nextcloud/spreed/pull/890)
  [#887](https://github.com/nextcloud/spreed/pull/887)

## 3.2.3 – 2018-07-11
### Changed
- Only paste the content of HTML into the chat input without the actual HTML 
  [#1018](https://github.com/nextcloud/spreed/pull/1018)

### Fixed
- Fixes for standalone signaling server
  [#910](https://github.com/nextcloud/spreed/pull/910)
- Name not shown for participants without audio and video
  [#982](https://github.com/nextcloud/spreed/pull/982)
- Correctly timeout users when they are chatting/calling and got disconnected 
  [#935](https://github.com/nextcloud/spreed/pull/935)
- Multiple layout fixes

## 3.2.2 – 2018-06-06
### Added
- Add toggle to show and hide video from other participants
  [#937](https://github.com/nextcloud/spreed/pull/937)

### Changed
- Activities and Notifications text (Calls->Conversations)
  [#919](https://github.com/nextcloud/spreed/pull/919)

### Fixed
- Send call notifications to every room participant that is not in the call
  [#926](https://github.com/nextcloud/spreed/pull/926)
- Mark messages directly as read when waiting for new messages
  [#936](https://github.com/nextcloud/spreed/pull/936)
- Fix tab header icons not shown
  [#929](https://github.com/nextcloud/spreed/pull/929)
- Fix room and participants menu buttons
  [#934](https://github.com/nextcloud/spreed/pull/934)
  [#941](https://github.com/nextcloud/spreed/pull/941)
- Fix local audio and video not disabled when not available
  [#938](https://github.com/nextcloud/spreed/pull/938)
- Fix "Add participant" shown to normal participants
  [#939](https://github.com/nextcloud/spreed/pull/939)
- Fix adding the same participant several times in a row
  [#940](https://github.com/nextcloud/spreed/pull/940)


## 3.2.1 – 2018-05-11
### Added
- Standalone signaling server now supports the 3.2 changes
  [#864](https://github.com/nextcloud/spreed/pull/864)
  [#869](https://github.com/nextcloud/spreed/pull/869)

### Fixed
- Only join the room after media permission request was answered
  [#854](https://github.com/nextcloud/spreed/pull/854)
- Do not reload the participant everytime a guest sends a chat message
  [#866](https://github.com/nextcloud/spreed/pull/866)
- Make sure the web UI still works after you left the current conversation or call
  [#871](https://github.com/nextcloud/spreed/pull/871)
  [#872](https://github.com/nextcloud/spreed/pull/872)
  [#874](https://github.com/nextcloud/spreed/pull/874)
- Allow to scroll on long participant lists again
  [#896](https://github.com/nextcloud/spreed/pull/896)
- Do not throw an error when starting a call in a conversation without any chat message
  [#861](https://github.com/nextcloud/spreed/pull/861)
- Enable media controls when media is approved on a second request
  [#861](https://github.com/nextcloud/spreed/pull/861)
- Limit the unread message counter to 99+
  [#845](https://github.com/nextcloud/spreed/pull/845)


## 3.2.0 – 2018-05-03
### Added
- Shortcuts have been added when a call is active: (m)ute, (v)ideo, (f)ullscreen, (c)hat and (p)articipant list
  [#730](https://github.com/nextcloud/spreed/pull/730)
  [#750](https://github.com/nextcloud/spreed/pull/750)
- Allow users to chat in multiple tabs in multiple chats at the same time
  [#748](https://github.com/nextcloud/spreed/pull/748)
- Guest names are now handled better in chat and the participant list
  [#733](https://github.com/nextcloud/spreed/pull/733)
- Users which are participanting in a call now have a video icon in the participant list
  [#777](https://github.com/nextcloud/spreed/pull/777)
- Unread chat message count is now displayed in the room list
  [#806](https://github.com/nextcloud/spreed/pull/806)
  [#824](https://github.com/nextcloud/spreed/pull/824)

### Changed
- It is now possible to join a call without camera and/or microphone
  [#758](https://github.com/nextcloud/spreed/pull/758)
- Chat does now not require Media permissions anymore
  [#711](https://github.com/nextcloud/spreed/pull/711)
- Leaving a call will free up the Media permissions
  [#735](https://github.com/nextcloud/spreed/pull/735)
- Participants can now be `@mentioned` in the chat by starting to type `@` followed by the name of the user
  [#805](https://github.com/nextcloud/spreed/pull/805)
  [#812](https://github.com/nextcloud/spreed/pull/812)
  [#813](https://github.com/nextcloud/spreed/pull/813)

### Fixed
- Correctly catch the input on the chat in firefox (instead of writing to the placeholder)
  [#737](https://github.com/nextcloud/spreed/pull/737)
- Keep scrolling position when switching from chat to call or back
  [#838](https://github.com/nextcloud/spreed/pull/838)
- Delete rooms when the last logged in user leaves
  [#727](https://github.com/nextcloud/spreed/pull/727)
- Correctly update chat UI when leaving current room
  [#743](https://github.com/nextcloud/spreed/pull/743)
- Various layout fixes with videos and screensharing
  [#702](https://github.com/nextcloud/spreed/pull/702)
  [#712](https://github.com/nextcloud/spreed/pull/712)
  [#713](https://github.com/nextcloud/spreed/pull/713)
- Fix issues with users that have a numerical name or id
  [#694](https://github.com/nextcloud/spreed/pull/694)
- Fix contacts menu entry when no user was found
  [#686](https://github.com/nextcloud/spreed/pull/686)


## 3.1.0 – 2018-02-14
### Added
- Finish support for go-based external signaling backend
  [#492](https://github.com/nextcloud/spreed/pull/492)

### Changed
- Make capabilities and signaling settings available for guests
  [#644](https://github.com/nextcloud/spreed/pull/644) [#654](https://github.com/nextcloud/spreed/pull/654)
- Use the search name as room name when creating a new room
  [#592](https://github.com/nextcloud/spreed/pull/592)
- Make links in chat clickable
  [#579](https://github.com/nextcloud/spreed/pull/579)

### Fixed
- Fix screensharing layout for guests
  [#611](https://github.com/nextcloud/spreed/pull/611)
- Correctly remember guest names when a guest is rejoining an existing call
  [#593](https://github.com/nextcloud/spreed/pull/593)
- Better date time divider in chat view
  [#591](https://github.com/nextcloud/spreed/pull/591)

## 3.0.1 – 2018-01-12
### Added
- Added capabilities so the mobile files apps can link to the mobile talk apps
  [#585](https://github.com/nextcloud/spreed/pull/585)

### Fixed
- Fixed issues when updating with Postgres and versions before 2.0.0
  [#584](https://github.com/nextcloud/spreed/pull/584)

## 3.0.0 – 2018-01-10
### Added
 - Added simple text chat
  [#429](https://github.com/nextcloud/spreed/pull/429)
 - Added activities for calls: "You had a call with ABC (Duration: 15:20)"
  [#438](https://github.com/nextcloud/spreed/pull/438)
 - Introduced different participant permission levels: owner, moderator and user
  [#353](https://github.com/nextcloud/spreed/pull/353)
 - Added support for room passwords on public shared rooms
  [#402](https://github.com/nextcloud/spreed/pull/402)
 - Added option to run an external signaling backend
  [#366](https://github.com/nextcloud/spreed/pull/366)

### Changed
 - Rename the app to "Talk" since it now contains chat, voice and video calls
  [#444](https://github.com/nextcloud/spreed/pull/444)
 - Moved admin settings to separate category and allowed to configure multiple STUN and TURN servers
  [#427](https://github.com/nextcloud/spreed/pull/427)
 - Moved signaling from EventSource to long polling for compatibility with HTTP2
  [#363](https://github.com/nextcloud/spreed/pull/363)
 - Moved room API to OCS so apps and 3rd party tools can use it
  [#342](https://github.com/nextcloud/spreed/pull/342)

### Fixed
 - Fixed compatibility with Postgres
  [#537](https://github.com/nextcloud/spreed/pull/537)
 - Fixed compatibility with Oracle
  [#371](https://github.com/nextcloud/spreed/pull/371)
 - Compatibility with Nextcloud 13


## 2.0.2 – 2017-11-28
### Fixed
 - Re-send data channels messages when they could not be sent.
  [#335](https://github.com/nextcloud/spreed/pull/335)

## 2.0.1 – 2017-05-22
### Added
 - Display the connection state in the interface and try to reconnect in case of an issue
  [#317](https://github.com/nextcloud/spreed/pull/317)

### Changed
 - Is now more tolerant towards server ping issues
  [#320](https://github.com/nextcloud/spreed/pull/320)

### Fixed
 - Fix several issues that caused missing avatars
  [#312](https://github.com/nextcloud/spreed/pull/312)
  [#313](https://github.com/nextcloud/spreed/pull/313)
 - Fix visibility of guest names on light themes
  [#321](https://github.com/nextcloud/spreed/pull/321)

## 2.0.0 – 2017-05-02
### Added
 - Screensharing is now supported in Chrome 42+ (requires an extension) and Firefox 52+
  [#227](https://github.com/nextcloud/spreed/pull/227)
 - Integration in the new Nextcloud 12 contacts menu
  [#300](https://github.com/nextcloud/spreed/pull/300)

### Changed
 - URLs are now short random strings instead of iteratible numbers
  [#258](https://github.com/nextcloud/spreed/pull/258)
 - Logged-in users can now join public rooms
  [#296](https://github.com/nextcloud/spreed/pull/296)

### Fixed
 - Fix error when response of TURN and STUN server arrive in the wrong order
  [#295](https://github.com/nextcloud/spreed/pull/295)


## 1.2.0 – 2017-01-18
### Added
 - Translations for multiple languages now available
  [#177](https://github.com/nextcloud/spreed/pull/177)
 - Open call-search when user has no calls
  [#111](https://github.com/nextcloud/spreed/pull/111)
 - Disable video by default, when more then 5 people are in a room

### Changed
 - TURN settings can only be changed by admins now
  [#185](https://github.com/nextcloud/spreed/pull/185)
 - App can not be restricted to groups anymore to prevent issues with public rooms
  [#201](https://github.com/nextcloud/spreed/pull/201)

### Fixed
 - Allow to connect via Firefox without a camera
  [#160](https://github.com/nextcloud/spreed/pull/160)
 - Leaving the current room does not refresh the full page anymore
  [#163](https://github.com/nextcloud/spreed/pull/163)
 - "Undefined index" log entry when visiting admin page
  [#151](https://github.com/nextcloud/spreed/pull/151)
  [#57](https://github.com/nextcloud/spreed/pull/57)


