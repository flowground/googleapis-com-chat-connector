# ![LOGO](logo.png) Hangouts Chat **flow**ground Connector

## Description

A generated **flow**ground connector for the Hangouts Chat API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/chat/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:16+03:00

## API Description

Enables bots to fetch information and perform actions in Hangouts Chat.

## Authorization

This API does not require authorization.

## Actions

### Lists spaces the caller is a member of.

*Tags:* `spaces`

#### Input Parameters
* `pageSize` - _optional_ - Requested page size. The value is capped at 1000.
Server may return fewer results than requested.
If unspecified, server will default to 100.
* `pageToken` - _optional_ - A token identifying a page of results the server should return.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Deletes a message.

*Tags:* `spaces`

#### Input Parameters
* `name` - _required_ - Required. Resource name of the message to be deleted, in the form
"spaces/*/messages/*"

Example: spaces/AAAAMpdlehY/messages/UMxbHmzDlr4.UMxbHmzDlr4
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns a message.

*Tags:* `spaces`

#### Input Parameters
* `name` - _required_ - Required. Resource name of the message to be retrieved, in the form
"spaces/*/messages/*".

Example: spaces/AAAAMpdlehY/messages/UMxbHmzDlr4.UMxbHmzDlr4
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Updates a message.

*Tags:* `spaces`

#### Input Parameters
* `name` - _required_ - Resource name, in the form "spaces/*/messages/*".

Example: spaces/AAAAMpdlehY/messages/UMxbHmzDlr4.UMxbHmzDlr4
* `updateMask` - _optional_ - Required. The field paths to be updated.

Currently supported field paths: "text", "cards".
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists human memberships in a space.

*Tags:* `spaces`

#### Input Parameters
* `pageSize` - _optional_ - Requested page size. The value is capped at 1000.
Server may return fewer results than requested.
If unspecified, server will default to 100.
* `pageToken` - _optional_ - A token identifying a page of results the server should return.
* `parent` - _required_ - Required. The resource name of the space for which membership list is to be
fetched, in the form "spaces/*".

Example: spaces/AAAAMpdlehY
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a message.

*Tags:* `spaces`

#### Input Parameters
* `parent` - _required_ - Required. Space resource name, in the form "spaces/*".
Example: spaces/AAAAMpdlehY
* `threadKey` - _optional_ - Opaque thread identifier string that can be specified to group messages
into a single thread. If this is the first message with a given thread
identifier, a new thread is created. Subsequent messages with the same
thread identifier will be posted into the same thread. This relieves bots
and webhooks from having to store the Hangouts Chat thread ID of a thread (created earlier by them) to post
further updates to it.

Has no effect if thread field,
corresponding to an existing thread, is set in message.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-chat-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
