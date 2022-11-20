# WinRar Password: kol2233

# Welcome 

EZFN.DEV is a free Fortnite Lobbybot which allows you to see all Fortnite cosmetics.

## Get Help
[Join my Discord](https://ezfn.dev/discord)

<sub>If you see this on github.com, visit [my website](https://ezfn.dev)...</sub>

# Fortnite: Save the World Daily Rewards Discord Bot

The official source code of the Discord Bot [STW Daily](https://discord.com/api/oauth2/authorize?client_id=757776996418715651&permissions=2147797056&scope=bot%20applications.commands), which can claim your STW daily reward. It is an adaptation of [this repository](https://github.com/Londiuh/fstwrc) by [Londiuh](https://github.com/Londiuh/).

## Important Information
### Using Public Hosted one:
Either [join the server](https://discord.gg/Mt7SgUu) or [invite the bot to your own server](https://discord.com/api/oauth2/authorize?client_id=757776996418715651&permissions=2147797056&scope=bot%20applications.commands), and run the commands you want. You can even do it in DMs with the bot if you want (but you need a mutual server with it).

### Self Hosting:
 - Clone the repo
 - Install the dependencies below
 - Add token for your bot as an environment variable for "STW_DAILY_TOKEN"
 - Invite your bot to your server
 - Run "daily core.py"

### Skids:
[Super easy 1-click hosting method](https://media.tenor.com/AKkrwSZSpZ0AAAPo/talking-ben.mp4)

### FAQ
You can read some commonly asked questions about the bot on the [STW Daily website](https://sites.google.com/view/stwdaily/docs/frequently-asked-questions)

## Requirements and dependencies
* Python 3 (Tested with 3.10.6)
* py-cord >= 2.1.1
* aiohttp < 3.9, >= 3.6.0
* psutil >= 5.9.1 
  * Only used in the "info" command. It is not essential to the functionality of the bot and can/should be removed; but you need to remove the code that uses it yourself.
* An Epic Games account with campaign access (Fortnite: Save the world)

You can install the required dependencies with:
```
pip install -r requirements.txt
```

## How to start the bot
Set your bot token as the value for the environment variable "STW_DAILY_TOKEN", then run "daily core.py"

If you don't know what a bot token is or need one, you can [create an application on discord](https://discord.com/developers/applications), then create a bot and copy it's token.

Alternatively, you can [Use my publicly one hosted on heroku here.](https://discord.com/api/oauth2/authorize?client_id=757776996418715651&permissions=2147797056&scope=bot%20applications.commands)

You can also [join my server](https://discord.gg/Mt7SgUu) if you would prefer to use the bot that way.

![STW Dailies Discord Invite](https://discordapp.com/api/guilds/757765475823517851/widget.png?style=banner2 "Discord Server Banner")

## How to use the bot
### @STW Daily {command} method
To interact with STW Daily, start your message by mentioning the bot (STW Daily), followed by the command you wish to use. For example, to authenticate and claim a daily reward, you will now run `@STW Daily d {code}`, instead of `stw d {code}`. Please note the space between the mention and the command.

You can learn more about all the new features and interactions STW Daily can provide by using `@STW Daily help`.
### / Slash command method
To get started with slash commands, start by typing `/`. You can learn more about slash commands [here](https://discord.com/blog/slash-commands-are-here).

How to get a code
---
To get an auth code [visit this website](https://www.epicgames.com/id/logout?redirectUrl=https%3A%2F%2Fwww.epicgames.com%2Fid%2Flogin%3FredirectUrl%3Dhttps%253A%252F%252Fwww.epicgames.com%252Fid%252Fapi%252Fredirect%253FclientId%253Dec684b8c687f479fadea3cb2ad83f5c6%2526responseType%253Dcode) and sign in with your Epic Games account.

You will then be taken to an empty webpage, with your authcode being displayed at the top left. 

```js
{"redirectUrl":"https://accounts.epicgames.com/fnauth?code=a51c1f4d35b1457c8e34a1f6026faa35","authorizationCode":"a51c1f4d35b1457c8e34a1f6026faa35","sid":null}
```

Copy only the authorisation code (you can double-click it in most browsers), and then add that to your command.

``@STW Daily d a51c1f4d35b1457c8e34a1f6026faa35``

The auth code will expire shortly after issued, and if used by STW Daily, will immediately expire. If you require a new code, you can simply [refresh the page](https://www.epicgames.com/id/api/redirect?clientId=ec684b8c687f479fadea3cb2ad83f5c6&responseType=code) to get a new code.

**NEW** in STW Daily beta: Authentication Sessions! Your authentication session will be saved for ~8 hours, allowing you to claim a daily, claim your research points and spend them without needing a new code each time. You will still need to provide a new code when the authentication session expires. You can opt out of automatically starting an authentication session by specifying any text after your auth code, e.g. `@STW Daily d a51c1f4d35b1457c8e34a1f6026faa35 no`. You can end an authentication session with `@STW Daily kill`

## Support
If you require assistance, just want to chat, or would prefer to use the bot in a different server to your own, you can [join the STW Daily discord](https://discord.gg/Mt7SgUu). Feel free to reach out directly to us via the server.

## Credits
[Londiuh](https://github.com/Londiuh) for their [code to collect daily rewards](https://github.com/Londiuh/fstwrc)

[Epic Research](https://github.com/MixV2/EpicResearch/)

Icons by [dippyshere ;)](https://github.com/dippyshere)

## Info
A valid auth token can be used maliciously, even though it expires when used, be careful, if you would like, you can [read more here](https://sites.google.com/view/stwdaily/docs/frequently-asked-questions) 

###### <p align=center> Portions of the materials used are trademarks and/or copyrighted works of Epic Games, Inc. </p>
###### <p align=center> All rights reserved by Epic. </p>
###### <p align=center> This material is not official and is not endorsed by Epic. </p>
###### <p align=center> All badges/icons (except the "Llama Calendar") are original copyrighted works by the author. </p>

# Saturn
This repo contains the code to build the Saturn Backend and Client for all supported platforms, as well as the source to the file provider [(`CUE4Parse`)](https://github.com/FabianFG/CUE4Parse).

## What is Saturn?
Saturn is the most advanced Fortnite Skin Changer on the market right now and it is completely free! Items get automatically added when EPIC adds them to Fortnite allowing you to change skins without having to wait for a contributor to add them to the program. The UI is also made in HTML, CSS, and JavaScript combining the smooth navigation of a website with the benefits of a native app.

Official Get-Started Page: https://github.com/Tamely/SaturnSwapper/blob/master/docs/using/GetStarted.md

## How can I contribute?
We welcome all kinds of contributions! Many people, listed or not, have bettered this project, and without them, it wouldn't be where it is today.

* [Contributing](docs/contributing/GetStarted.md) explains what kind of contributions we welcome
* [Workflow Instructions](docs/contributing/BuildingAndRunning.md) explains how to build and run the project
* [Fortnite's File Documentation](docs/contributing/FortniteFiles.md) gives a quick overview of where everything is located in Fortnite's files and how Saturn takes advantage of it

## Reporting security issues and security bugs

Security issues and bugs should be reported privately, via DM on Discord, to any Admin/Contributor role holder in [Saturn's Discord](https://discord.gg/Saturn). You should receive a response within 24 hours. If - for whatever reason - you do not, please DM Tamely#6469 directly. You may be entitled to financial compensation for your report depending on the severity of the issue.

## Filing issues

This repo should contain issues that are tied to the actual codebase of the project. If a feature of the project is not working as intended, please use the `Support` channel in [Saturn's Discord](https://discord.gg/Saturn) to resolve your issue.

## Useful Links
* [Saturn's Discord](https://discord.gg/Saturn)
* [.NET 6 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.0-windows-x64-installer) - Needed for running the project
* [WebView2 Runtime (comes with Windows 11, you need the x64 Evergreen Bootstrapper)](https://developer.microsoft.com/en-us/microsoft-edge/webview2/#download-section) - Needed to run the website the project hosts as a native program

## Unlisted Contributors

| Contributor | Contribution |
| ----------- | ----------- |
| [Amr Satrio](https://github.com/Amrsatrio)   | Helped with asset obfuscation and just general questions |
| [cyclonefreeze](https://github.com/cyclonefreeze)   | Developed base which Saturn built upon |
| [jakedothow](https://github.com/jakedothow)   | Developed base which Saturn built upon |
| [All CUE4Parse contributors](https://github.com/FabianFG/CUE4Parse/graphs/contributors)   | CUE4Parse is the main part of the swapper |

## License

Saturn is license under the [GNU General Public License v3.0](LICENSE)

[![FTNPower Discord Bot](https://top.gg/api/widget/lib/454547389731045380.svg)](https://top.gg/bot/454547389731045380) [![FTNPower Servers](https://top.gg/api/widget/servers/454547389731045380.svg)](https://top.gg/bot/454547389731045380) [![FTN Power Owner](https://top.gg/api/widget/owner/454547389731045380.svg)](https://top.gg/bot/454547389731045380)
# FTN Power
Source codes of the FTN Power project have been published (including private Fortnite STW API and services), feel free to use. FTN Power discord bot has been shut down. Thank you for all your supports.

| FTN Power Libraries      |
| :---        |
| [Fortnite STW API](https://github.com/msx752/FTN-Power/tree/master/src/Fortnite)      |
| [Fortnite Power Level Formula](https://github.com/msx752/FTN-Power/blob/master/src/Tests/FortniteLib.Tests/UserUnit.cs#L44)      |
| [Fortnite Assets](https://raw.githubusercontent.com/msx752/FTN-Power/master/RequiredVolumeData/fortnite-volume/_data/FTNPower/_CDNIMGIDS.json)      |
| [FTN Power discord bot](https://github.com/msx752/FTN-Power/tree/master/src/FTNPowerApplication)      |
| [FTN Power back-end services](https://github.com/msx752/FTN-Power/tree/master/src/FortnitePowerQueue)      |
| [FTN Power image service](https://github.com/msx752/FTN-Power/tree/master/src/Websites/FTNPower.Image.Api)     |
| [FTN Power redis service](https://github.com/msx752/FTN-Power/tree/master/src/RedisDockerfile)      |
| [FTN Power log service](https://github.com/msx752/FTN-Power/tree/master/src/SeqDockerfile)      |
| [FTN Power logger](https://github.com/msx752/FTN-Power/tree/master/src/GlobalLibs/MyLogger)      |

[![FTN Power Commands](https://raw.githubusercontent.com/msx752/FTN-Power/master/ftnpower-discordbot.png)](https://github.com/msx752/FTN-Power)

# ApexD3D_External
Apex Legends External Hack








[![Maven Central](https://img.shields.io/maven-central/v/io.github.robertograham/fortnite-2-xmpp.svg?label=Maven%20Central&style=flat-square)](https://search.maven.org/search?q=g:%22io.github.robertograham%22%20AND%20a:%22fortnite-2-xmpp%22)

# fortnite-2-xmpp

A Java 11+ client for Fortnite's XMPP services

## Features

* Ability to send chat messages and process inbound chat messages
* Ability to process friends list received after connecting
* Ability to process friends' presence updates

## Installation

### Maven

```xml
<properties>
  ...
  <!-- Use the latest version whenever possible. -->
  <fortnite-2-xmpp.version>1.0.0</fortnite-2.version>
  ...
</properties>

<dependencies>
  ...
  <dependency>
    <groupId>io.github.robertograham</groupId>
    <artifactId>fortnite-2-xmpp</artifactId>
    <version>${fortnite-2-xmpp.version}</version>
  </dependency>
  ...
</dependencies>
```

## Usage

### Instantiating a client

This is the simplest way to instantiate a client:

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

public final class Main {

    public static void main(final String[] args) {
        final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
            .build();
        final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
            .build();
    }
}
```

By default fortnite-2-xmpp will not debug raw XMPP traffic but this can be enabled like so:

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

public final class Main {

    public static void main(final String[] args) {
        final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
            .build();
        final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
            .setDebugXmppConnections(true)
            .build();
    }
}
```

The platform and application the authenticated user is using can be spoofed like so:

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

public final class Main {

    public static void main(final String[] args) {
        final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
            .build();
        final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
            .setApplication(Application.FORTNITE_CLIENT)
            .setPlatform(Platform.NINTENDO_SWITCH)
            .build();
    }
}
``` 

### Cleaning up

When you no longer need your client instance, remember to close your XMPP connections with a call to `FortniteXmpp.close()`. Usage examples further in this document will make 
this call implicitly using `try`-with-resources statements.

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

public final class Main {

    public static void main(final String[] args) {
        final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
            .build();
        final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
            .build();
        fortniteXmpp.close();
        fortnite.close();
    }
}
```

### Listeners

Register an `OnFriendsListReceivedListener` that prints the `Account` representation of every friend

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

import java.io.IOException;

public final class Main {

    public static void main(final String[] args) {
        try (
            final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
                .build();
            final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
                .setOnFriendsListReceivedListener((final var accountIds, final var friend) -> {
                    try {
                        fortnite.account()
                            .findAllByAccountIds(accountIds.toArray(String[]::new))
                            .ifPresent((final var accounts) -> accounts.forEach(System.out::println));
                    } catch (final IOException exception) {
                        // findAllByAccountIds unexpected response
                    }
                })
                .build()
        ) {
        }
    }
}
```

Register an `OnFriendPresenceReceivedListener` that stores friends and their presence details in a `Map`

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.domain.Session;
import io.github.robertograham.fortnite2.xmpp.domain.enumeration.Status;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

import java.util.AbstractMap.SimpleEntry;
import java.util.HashMap;
import java.util.Map.Entry;

public final class Main {

    public static void main(final String[] args) {
        final var accountIdToStatusSessionEntryMap = new HashMap<String, Entry<Status, Session>>();
        try (
            final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
                .build();
            final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
                .setOnFriendPresenceReceivedListener((final var accountId, final var status, final var sessionOptional, final var friend) ->
                    accountIdToStatusSessionEntryMap.put(accountId, new SimpleEntry<>(status, sessionOptional.orElse(null)))
                )
                .build()
        ) {
            while (accountIdToStatusSessionEntryMap.isEmpty())
                System.out.println("Awaiting presence");
            accountIdToStatusSessionEntryMap.forEach((final var accountId, final var statusToSessionEntry) ->
                System.out.printf("%s[%s]: %s\n", accountId, statusToSessionEntry.getKey(), statusToSessionEntry.getValue())
            );
        }
    }
}
```

### Chat API

Register an `OnChatMessageReceivedListener`, send a message to the authenticated account and wait for the message to be self-received

```java
import io.github.robertograham.fortnite2.implementation.DefaultFortnite;
import io.github.robertograham.fortnite2.xmpp.implementation.DefaultFortniteXmpp;

import java.io.IOException;

public final class Main {

    public static void main(final String[] args) {
        try (
            final var fortnite = DefaultFortnite.Builder.newInstance("epicGamesEmailAddress", "epicGamesPassword")
                .build();
            final var fortniteXmpp = DefaultFortniteXmpp.Builder.newInstance(fortnite)
                .setOnChatMessageReceivedListener((final var accountId, final var messageBody, final var chat) ->
                    System.out.printf("New message from %s!%n", accountId)
                )
                .build()
        ) {
            final var sessionAccount = fortnite.account()
                .findOneBySessionAccountId()
                .orElseThrow();
            fortniteXmpp.chat()
                .sendMessageToAccount(sessionAccount, "WE LOVE FORTNITE WE LOVE FORTNITE");
            while (fortniteXmpp.chat()
                .findAllMessagesReceivedFromAccount(sessionAccount)
                .isEmpty()) ;
            fortniteXmpp.chat()
                .findAllMessagesReceivedFromAccount(sessionAccount)
                .forEach(System.out::println);
        } catch (final IOException exception) {
            // findOneBySessionAccountId unexpected response
            // OR sendMessageToAccount failed
        }
    }
}
```