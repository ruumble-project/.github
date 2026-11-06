# Ruumble

**Your [Mumble](https://www.mumble.info/) server as an office building.**

Ruumble turns the channels of a Mumble server into floors and rooms. You see at a glance who sits where and who is talking, you move to another room with a click, and every room has a board for notes, code, images and files. Voice stays in Mumble, and Mumble itself stays unchanged.

[![Server release](https://img.shields.io/github/v/release/ruumble-project/ruumble-server?label=server)](https://github.com/ruumble-project/ruumble-server/releases/latest) [![Client release](https://img.shields.io/github/v/release/ruumble-project/ruumble-client?label=client)](https://github.com/ruumble-project/ruumble-client/releases/latest) [![What's new](https://img.shields.io/badge/what's%20new-release%20notes-0078be)](https://github.com/ruumble-project/ruumble-server/blob/main/docs/whats-new/README.md)

![Ruumble: moving between rooms, a new post on the board, the elevator and back via the room sign](https://raw.githubusercontent.com/ruumble-project/ruumble-server/main/docs/images/ruumble-demo.gif)

## Is Ruumble for you?

Ruumble is made for teams that already talk in Mumble all day, or want to, and miss the feeling of a shared office: who is around, who is busy, where can I drop in.

- **It is an add-on, not a standalone app.** It needs a Mumble server that you run or administer. The server operator runs one small Docker container next to it.
- **Users** use **Ruumble Client**, a Mumble client with Ruumble built in (Linux), or the **Ruumble plugin** in their own Mumble client (Linux and Windows) together with a browser.
- **Plain Mumble keeps working.** People without Ruumble join the same channels as before; Ruumble only reads the server and changes nothing in Mumble's setup.

| You need | |
|---|---|
| Mumble server | 1.5 or newer, with Ice enabled |
| Service | Docker, network access to the Mumble server's Ice port |
| Ruumble Client | Linux (x86_64): AppImage, .deb, .rpm or Arch package |
| Or the plugin | Mumble 1.4 or newer on Linux (x86_64) or Windows (x64), plus a current Firefox, Chrome or Edge |

## What you get

- **The building:** top-level channels become floors, the channels below them rooms, the floor channel itself the corridor. An elevator takes you to the other floors, a building overview shows everyone at once.
- **Presence:** who is talking, muted or deafened, quiet or away, a short status text, recording and listeners, Mumble avatars.
- **One click to move:** Ruumble moves your Mumble client; mute and deafen work from Ruumble too.
- **A board in every room:** Markdown, source code, images and files, reactions, shared task lists, search.
- **Talk without talking:** a quiet word in private, files handed straight to a person or a room (tube mail), a nudge for someone who is deafened.
- **Care for admins:** set up rooms and floors, tidy up old posts and boards, revoke paired browsers, all from Ruumble.
- **German and English.**

The full list: [features](https://github.com/ruumble-project/ruumble-server/blob/main/docs/features.md).

## Get started

- **Server operators:** three commands with Docker, in the [ruumble-server README](https://github.com/ruumble-project/ruumble-server#get-started).
- **Users on Linux:** download Ruumble Client from the [latest client release](https://github.com/ruumble-project/ruumble-client/releases/latest) and connect to your server. It offers to take over an installed Mumble with its certificate and servers.
- **Users with their own Mumble client:** install the plugin, see the [user guide](https://github.com/ruumble-project/ruumble-server/blob/main/docs/user-guide.md).

## What's new

The [release notes for users](https://github.com/ruumble-project/ruumble-server/blob/main/docs/whats-new/README.md) tell what changed in each version, in plain words and with pictures, the newest version on top. [Coming next](https://github.com/ruumble-project/ruumble-server/blob/main/docs/whats-new/next.md) shows what is already done for the next one.

Releases: [server](https://github.com/ruumble-project/ruumble-server/releases/latest) (Docker image, plugin, Compose templates) and [Ruumble Client](https://github.com/ruumble-project/ruumble-client/releases/latest). Both have their own version numbers, and any client works with older and newer servers.

## For developers and the team

> [!IMPORTANT]
> **[Open the team Kanban board](https://github.com/orgs/ruumble-project/projects/1)**: tickets of ruumble-client and ruumble-server, who works on what and the status of each.
> You need access to the Ruumble organization; if the page shows a 404, ask a maintainer to add you to the board.

| Repository | |
|---|---|
| [**ruumble-server**](https://github.com/ruumble-project/ruumble-server) | The service (one Docker container), the web UI and the Mumble plugin. Build, test and architecture start here. |
| [**ruumble-client**](https://github.com/ruumble-project/ruumble-client) | Ruumble Client: a Mumble 1.6 client for Linux with Ruumble built in. One window, no plugin and no browser tab. |

Questions, ideas, bugs and feature requests: issues in either repository. Contributions are welcome, see [CONTRIBUTING](https://github.com/ruumble-project/ruumble-server/blob/main/CONTRIBUTING.md).

Ruumble is open source under the BSD-3-Clause license. It is not affiliated with or endorsed by the Mumble project.
