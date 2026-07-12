+++
date = '2026-07-12T21:36:16+10:00'
draft = true
title = 'Updating my Password Manager'
+++

Well it finally happened. I was pretty sure it was going to, I just didn't know when.

My trusty [KeePassX](https://www.keepassx.org/) solution was EOL.  Apple announcing the retirement of Rosetta meant KeepPassX was going to stop working.  I didnt actually realise KeePassX had no longer been in active development since 2021 so it was definetly time for a change.

I been keeping my passwords in a KeePass 1 database file stored in my google drive since 2014. I use KeePassDroid on my phone and KeePassX on my MacBooks.  It worked for me really well and I felt happy I wasnt subject of any of the cloud data breaches that were happening at the time and since.

Anyway, what to replace KeePass with? I still wanted to self host and have on my phone.  An added bonus would be a chrome plugin to enter passwords into website would be great.

My search led me to [this reddit thread](https://www.reddit.com/r/selfhosted/comments/1pwwjm4/selfhostable_opensource_password_managers_2025/).  Some good options in there that I had never heard of.

## [Self-host Bitwarden](https://bitwarden.com/help/self-host-bitwarden/)
I didnt realise companies like Bit Warden would let you run your own instance of their app.  Any for free too!  Lots of advantages like Web based, Chrome Extension, Android App.

The downside is you need you make the "server" publically accessible so the android app can get access to your passwords. 

## [Self-host Passbolt](https://www.passbolt.com/ce/docker)
Similar deal, self host in Docker, android app and chrome extension.

Same downside, you need to self host, domain, ssl etc.

## [Psono](https://psono.com/)
This one is the same, but seems to be designed first for self hosting with cloud hosting as an additional option.

Sode note; I do find it a little scary that all these are free.  One would assume the open source community is going to keep on top of any scary security holes in these apps.

The biggest thing with these options for me is ensuring whatever platform I hosted these on is secure and not going to leak all my passwords to the internet.  Also I have enough Raspberry PIs here, I dont really want any more!

I'm glad I took the time to look at other options.  If I had more of a need to share passwords with family etc then I would give Psono a crack I think.  I will certainly be mentioning it to my boss because we are in desperate need for a password management solution specifically for shared passwords.

I opted for the direct drop in [KeePasssXC](https://keepassxc.org/) to replace KeePass.  Had to upgrade my kdb to kdbx file, but other than that, works natively on OSX, has some kind of web server in it which connects to a chrome extension and I can keep using [KeePassDroid](https://play.google.com/store/apps/details?id=com.android.keepass&hl=en_AU) on my phone.