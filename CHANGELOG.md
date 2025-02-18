## [1.4.5](https://github.com/peers/peerjs/compare/v1.4.4...v1.4.5) (2022-05-24)


### Bug Fixes

* **referrerPolicy:** you can now set a custom referrerPolicy for api requests ([c0ba9e4](https://github.com/peers/peerjs/commit/c0ba9e4b64f233c2733a8c5e904a8536ae37eb42)), closes [#955](https://github.com/peers/peerjs/issues/955)
* **typings:** add missing type exports ([#959](https://github.com/peers/peerjs/issues/959)) ([3c915d5](https://github.com/peers/peerjs/commit/3c915d57bb18ac822d3438d879717266ee84b635)), closes [#961](https://github.com/peers/peerjs/issues/961)

## [1.4.4](https://github.com/peers/peerjs/compare/v1.4.3...v1.4.4) (2022-05-13)


### Bug Fixes

* **CRA@4:** import hack ([41c3ba7](https://github.com/peers/peerjs/commit/41c3ba7b2ca6adc226efd0e2add546a570a4aa3a)), closes [#954](https://github.com/peers/peerjs/issues/954)
* **source maps:** enable source map inlining ([97a724b](https://github.com/peers/peerjs/commit/97a724b6a1e04817d79ecaf91d4384ae3a94cf99))

## [1.4.3](https://github.com/peers/peerjs/compare/v1.4.2...v1.4.3) (2022-05-13)


### Bug Fixes

* **typings:** export interfaces ([979e695](https://github.com/peers/peerjs/commit/979e69545cc2fe10c60535ac9793140ef8dba4ec)), closes [#953](https://github.com/peers/peerjs/issues/953)

## [1.4.2](https://github.com/peers/peerjs/compare/v1.4.1...v1.4.2) (2022-05-12)


### Bug Fixes

* **bundler import:** enable module target ([b5beec4](https://github.com/peers/peerjs/commit/b5beec4a07827f82c5e50c79c71a8cfb1ec3c40e)), closes [#761](https://github.com/peers/peerjs/issues/761)

## [1.4.1](https://github.com/peers/peerjs/compare/v1.4.0...v1.4.1) (2022-05-11)


### Bug Fixes

* **old bundlers:** include support for Node 10 (EOL since 2021-04-01) / old bundlers ([c0f4648](https://github.com/peers/peerjs/commit/c0f4648b1c104e5e0e5967bb239c217288aa83e0)), closes [#952](https://github.com/peers/peerjs/issues/952)

# [1.4.0](https://github.com/peers/peerjs/compare/v1.3.2...v1.4.0) (2022-05-10)


### Bug Fixes

* add changelog and npm version to the repo ([d5bd955](https://github.com/peers/peerjs/commit/d5bd9552daf5d42f9d04b3087ddc34c729004daa))
* add token to PeerJSOption type definition ([e7675e1](https://github.com/peers/peerjs/commit/e7675e1474b079b2804167c70335a6c6e2b8ec08))
* websocket connection string ([82b8c71](https://github.com/peers/peerjs/commit/82b8c713bc03be34c2526bdf442a583c4d547c83))


### Features

* upgrade to Parcel@2 ([aae9d1f](https://github.com/peers/peerjs/commit/aae9d1fa37731d0819f93535b8ad78fe4b685d1e)), closes [#845](https://github.com/peers/peerjs/issues/845) [#859](https://github.com/peers/peerjs/issues/859) [#552](https://github.com/peers/peerjs/issues/552) [#585](https://github.com/peers/peerjs/issues/585)


### Performance Improvements

* **turn:** lower TURN-latency due to more local servers ([a412ea4](https://github.com/peers/peerjs/commit/a412ea4984a46d50de8873904b7067897b0f29f9))

<a name="1.3.2"></a>

## 1.3.2 (2021-03-11)

- fixed issues #800, #803 in PR #806, thanks @jordanaustin
- updated devDeps: `typescript` to 4.2

<a name="1.3.1"></a>

## 1.3.1 (2020-07-11)

- fixed: map file resolving
- removed: @types/webrtc because it contains in ts dom lib.

<a name="1.3.0"></a>

## 1.3.0 (2020-07-03)

- changed: don't close the Connection if `iceConnectionState` changed to `disconnected`

<a name="1.2.0"></a>

## 1.2.0 (2019-12-24)

- added: ability to change json stringify / json parse methods for DataConnection #592

- removed: `peerBrowser` field from `dataConnection` because unused

- fixed: lastServerId and reconnect #580 #534 #265

<a name="1.1.0"></a>

## 1.1.0 (2019-09-16)

- removed: deprecated `RtpDataChannels` and `DtlsSrtpKeyAgreement` options
- removed: grunt from deps, upgrade deps versions
- removed: Reliable dep because modern browsers supports `RTCDataChannel.ordered` property

- added: TURN server to default config

- fixed: emit error message, then destory/disconnect when error occured
- fixed: use `peerjs-js-binarypack` instead of `js-binarypack`
- fixed: sending large files via DataConnection #121

<a name="1.0.4"></a>

## 1.0.4 (2019-08-31)

- fixed: 'close' event for DataConnection #568

<a name="1.0.3"></a>

## 1.0.3 (2019-08-21)

- add pingInterval option

<a name="1.0.2"></a>

## 1.0.2 (2019-07-20)

### Bug Fixes

- fixed: memory leak in DataConnection #556
- fixed: missing sdpMid in IceServer #550

### Other

- updated: old @types/webrtc dependency #549

<a name="1.0.1"></a>

## 1.0.1 (2019-07-09)

### Bug Fixes

- fixed: readyState of undefined #520
- fixed: call sdpTransform in Answer #524
- fixed: sdpTransform does not apply to makeAnswer SDP #523

<a name="1.0.0"></a>

## 1.0.0 (2019-04-10)

### Refactoring

Almost all project was refactored!!!

- removed: xhr long-pooling #506
- changed: fetch api instead of xhr

### Features

- added: heartbeat #502

### Bug Fixes

- fixed: destroy RTCPeerConnection #513
- fixed: MediaStream memory leak #514

<a name="0.3.18"></a>

## 0.3.18 (2018-10-30)

### Features

- **typescript:** First commit ([0c77a5b](https://github.com/peers/peerjs/commit/0c77a5b))

<a name="0.3.16"></a>

## 0.3.16 (2018-08-21)

### Bug Fixes

- fixed typo in README ([f1bd47e](https://github.com/peers/peerjs/commit/f1bd47e))

## Version 0.3.14

- Patch for #246, which started as of Chrome 38.

## Version 0.3.11 (28 Sep 2014)

- Browserify build system

## Version 0.3.10 (29 Aug 2014)

- Fixed a bug where `disconnected` would be emitted for XHR requests that were aborted on purpose.

## Version 0.3.9 (11 July 2014)

- Allow an external adapter to be used (for `RTCPeerConnection` and such). (Thanks, @khankuan!)
- Fixed a bug where `_chunkedData` was not being cleared recursively, causing memory to be eaten up unnecessarily. (Thanks, @UnsungHero97!)
- Added `peer.reconnect()`, which allows a peer to reconnect to the signalling server with the same ID it had before after it has been disconnected. (Thanks, @jure, for the amazing input :)!)
- Added previously-missing error types, such as `webrtc`, `network`, and `peer-unavailable` error types. (Thanks, @mmis1000 for reporting!)
- Fixed a bug where the peer would infinitely attempt to start XHR streaming when there is no network connection available. Now, the peer will simply emit a `network` error and disconnect. (Thanks, @UnsungHero97 for reporting!)

## Version 0.3.8 beta (18 Mar 2014)

- **The following changes are only compatible with PeerServer 0.2.4.**
- Added the ability to specify a custom path when connecting to a self-hosted
  PeerServer.
- Added the ability to retrieve a list of all peers connected to the server.

## Version 0.3.7 beta (23 Dec 2013)

- Chrome 31+/Firefox 27+ DataConnection interop for files.
- Deprecate `binary-utf8` in favor of faster support for UTF8 in the regular
  `binary` serialization.
- Fix `invalid-key` error message.

## Version 0.3.6 beta (3 Dec 2013)

- Workaround for hitting Chrome 31+ buffer limit.
- Add `.bufferSize` to DataConnection to indicate the size of the buffer queue.
- Add `.dataChannel` to DataConnection as an alias for `._dc`, which contains
  the RTCDataChannel object associated with the DataConnection.
- Update BinaryPack dependency.

## Version 0.3.5 beta (26 Nov 2013)

- Fix bug where chunks were being emitted.

## Version 0.3.4 beta (11 Nov 2013)

- Fix file transfer issue in Chrome by chunking for data over 120KB.
- Use binary data when possible.
- Update BinaryPack dependency to fix inefficiencies.

## Version 0.3.3 beta (2 Nov 2013)

- Fix exceptions when peer emits errors upon creation
- Remove extra commas

## Version 0.3.2 beta (25 Oct 2013)

- Use SCTP in Chrome 31+.
- Work around Chrome 31+ tab crash. The crashes were due to Chrome's lack of support for the `maxRetransmits` parameter for modifying SDP.
- Fix exceptions in Chrome 29 and below.
- DataChannels are unreliable by default in Chrome 30 and below. In setting
  reliable to `true`, the reliable shim is used only in Chrome 30 and below.

## Version 0.3.1 beta (19 Oct 2013)

- Updated docs and examples for TURN server usage
- Fixed global variable leak
- DataConnections now have reliable: false by default. This will switch to on when reliable: true works in more browsers

## Version 0.3.0 beta (20 Sept 2013)

### Highlights

- Support for WebRTC video and audio streams in both Firefox and Chrome.
- Add `util.supports.[FEATURE]` flags, which represent the WebRTC features
  supported by your browser.
- **Breaking:** Deprecate current `Peer#connections` format. Connections will no longer be
  keyed by label and will instead be in a list.

### Other changes

- **Breaking:** Deprecate `Peer.browser` in favor of `util.browser`.
- Additional logging levels (warnings, errors, all).
- Additional logging functionality (`logFunction`).
- SSL option now in config rather than automatic.

## Version 0.2.8 (1 July 2013)

- Fix bug, no error on Firefox 24 due to missing error callback.
- TLS secure PeerServers now supported.
- Updated version of Reliable shim.

## Version 0.2.7 (28 May 2013)

- Fix bug, no error when .disconnect called in before socket connection established.
- Fix bug, failure to enter debug mode when aborting because browser not supported.

## Version 0.2.6 (2 May 2013)

- Peer.browser to check browser type.
- Update Reliable library and fix Reliable functionality in Chrome.

## Version 0.2.5 (24 Apr 2013)

- **Firefox compatibility for Firefox Nightly.**
- Misc bug fixes.

## Version 0.2.1 (3 Apr 2013)

- **Warning**: this build changes the error of type `peer-destroyed` to `server-disconnected`.
- ~~**Firefox compatibility.**~~ - Pushed back due to volatility of Firefox Nightly DataChannel APIs.
- Browser detection added. If an incompatible browser is detected, the `browser-incompatible` error is emitted from the `Peer`.
- Added a `.disconnect()` method to `Peer`, which can be called to close connections to the PeerServer (but not any active DataConnections).

## Version 0.2.0 (24 Mar 2013)

- **Warning**: this build introduces the following API changes that may break existing code.
  - `peer.connections` is no longer a hash mapping peer IDs to connections.
  - Connections no longer emit errors from `PeerConnection`; `PeerConnection` errors are now forwarded to the `Peer` object.
- Add support for multiple DataConnections with different labels.
- Update Reliable version to support faster file transfer.
- Fix bug where using XHR streaming to broker a connection occasionally fails.

## Version 0.1.7 (6 Mar 2013)

- Add experimental `reliable` messaging option. [See documentation.](https://github.com/peers/peerjs/blob/master/docs/api.md#experimental-reliable-and-large-file-transfer)
- Fix bug where the ID /GET request was cached and so two Peers created simultaneously would get the same ID: [See issue.](https://github.com/peers/peerjs-server/issues/2)
- Add support for relative hostname. [See documentation.](https://github.com/peers/peerjs/blob/master/docs/api.md#new-peerid-options)
