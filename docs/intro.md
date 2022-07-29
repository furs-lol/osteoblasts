---
sidebar_position: 1
---

*Everything is subject to change*

# Getting started with the API

The Furs-lol (Not final name -- Only the current project name) API is not open for public use, yet. We will have a public beta when we are 
ready for users to start using our service. You can join our [Discord server](https://discord.gg/GFWaxnNXyt) for some updates on development.
When we do have a public beta an invite will be posted in our server for people to use (Details on this are still blurry.)

None the less these docs will go over the API for internal use. User bots (User accounts automated by programs) are not currently allowed
and may never be allowed.

## Errors

:::warning
I am still in the process of making all routes return proper errors.
:::

Errors from the API will return a message and code. You can find the code in our [resource page about errors](/docs/intro.md). Below is an
example of an error returned from the API
```json
{
  "message": "You're not permitted to view this account.",
  "code": 40001
}
```