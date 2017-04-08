# gdx-remote-tv

My attempt to build a *TV guide & remote control* app which doesn't blow. Let's see how this works out...

## rant

I own a Sony Bravia TV, which is a nice piece of hardware, but operating it via remote is an awkward experience. The operating system they use on these devices is slow as hell. The user experience is just awful.

For this reason, I've been using the "Sony TV SideView" Android app for the past few years. Now, user experience wise, this app is just a huge pile of steaming crap itself. Unfortunately, it's been the best I could find, plus it features a TV program guide synchronized to my cable TV channel list. So, I'm able to "comfortably" use an Android device to browse the TV program and switch channels.

Now, it seems Sony didn't manage to shove enough money down the throat of whoever is in charge of this application and/or their partners, and, in all their glorious wisdom, decided to pull the plug. Which means that, end of May 2017, they'll cut anything "remotely" (pun intended) useful from their app, only leaving features I don't need.

## feature wish list

- a program guide view to browse TV channels
  - "import" channel list from TV (how?)
- a means to import TV program information
  - through a provider plugin mechanism of some kind
  - currently looking into http://www.epgdata.com, though this is pay-to-use
  - possibly host this part on a server, e.g. my small RPi home server, to cron and aggregate source data
- remote command TV device
  - probably web based, Sony for example has some weird REST API built in
  - again, a plugin system of some sort to customize this part
  - a "macro" option to send arbitrary command chains (this is a rant for another day)