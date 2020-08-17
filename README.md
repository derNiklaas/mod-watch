## mod-watch

mod-watch is a plugin for [nodecg-io](https://nodecg-io), that allows a broadcaster to monitor the activity of their moderation team.

### Installation

1. Clone this project into an existing [nodecg-io](https://nodecg-io) installation.
2. Add the path to the mod-watch folder in the ``lerna.json`` file.
3. Edit the channel and the name of the bots in ``mod-watch/extension/index.ts``.
4. Run ``npm run bootstrap`` and ``npm run build`` in the nodecg-io directory.
5. Start nodecg, create a new Twitch instance and assign it to mod-watch.
Note: The Twitch account should have the following permissions: ``chat:read whispers:edit whispers:send``

### How to use mod-watch

The account you specified (it should NOT be your account) will now sit in your channel and listen for any messages from a moderator.

It will save the date of the last message in ``mod-watch/extension/data/data.json``.
The broadcaster can also use ``!mod-watch mods``.