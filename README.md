
## What this is not

A guidwork replacement.

Guildwork is still defect.

---

## What this is

A launcher for guildwork.exe

Some things like bazaar, merit/job points and titles are still working

---

## How To Install

- 1/ Download guildwork.exe from https://guildwork.s3.amazonaws.com/guildwork/Guildwork.exe

Copy guildwork.exe to ashita plugins folder

- 2/ Plugin install

Plugin has been compiled with VS 2022

Get runtimes at https://learn.microsoft.com/fr-fr/cpp/windows/latest-supported-vc-redist?view=msvc-170

Install x86 version

Copy guildwork.dll, Guildwork_zmq_S.exe and libzmq-v143-mt-4_3_6.dll to ashita plugins folder

---

## Usage

- /load guildwork

- /gw login {email} {password}

Need to be done 1 time only (credentials are saved in C:\Users\{username}\AppData\Roaming\Guildwork\settings.json)

- /gw flush

- /gw flush --add

- /gw exit or /unload guildwork

Others commands have not been implemented because i don't need them and i don't have a premium account to test.

---

## Config

Edit {ashita path}/config/guildwork/config.ini

By default, debug and outgoing packet are disabled

Enabling these 2 options are not mandatory to run the plugin

- Debug is just to see guildwork messages

- Outgoing packet is used to get job points faster

Same result could be achieve by opening job points menu

---

## Tips

Because i have done it wrong for several years on windower and ashita v3.

- Merit points are parsed at zoning

If you load the plugin and flush without zoning, merit points will not be flushed

The correct things to do are load the plugin, zone and then flush

You can check your merit points on guildwork.com and ffxiah.com sites

SE changes some of them years ago (Protectra V, Katon: San, Foe Sirvente... have been replaced by others)

They will not be displayed correctly on guildwork.com because it has not been updated, but ffxiah.com have them correctly

- Job points are parsed when you open job points menu

But the ffxi client request this only 1 time each time you zone and only if you open job points menu

If you zone, open the menu, load the plugin, job points will not be flushed, even if you open the job points menu again

The correct things to do are load the plugin, zone, open job points menu then flush



