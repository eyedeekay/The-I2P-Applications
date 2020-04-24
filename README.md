The-I2P-Applications
====================

Introduction
------------

When you install the I2P router as made available at [geti2p.net](https://geti2p.net/en/download),
you are actually installing an I2P router and an accompanying bundle of about a
dozen basic applications. These are all made available to the user via a webUI,
which listens at [127.0.0.1:7657](http://127.0.0.1:7657), and the main page of
which is called the "Router Console," where you monitor the health of all the
applications that are using I2P and navigate I2P configuration, control, and
feedback. This document, in order of significance to the new user, attempts to
elucidate the relationship between I2P, Applications Internal to I2P, and
Applications External to I2P, without going into too much detail about the areas
in-between.

Table of Contents
-----------------

- **Applications for *Users* to get started with**
 1. **[The I2P Router Console](http://localhost:7657/home):** This is the "Start Menu" of I2P where you get
  information about the running I2P router, configure the application settings,
  and find shortcuts to other applications. Over the years, it has evolved
  considerable customizability.
 2. **[I2P Hidden Services Manager](http://localhost:7657/i2ptunnelmgr):** This is a general-purpose adapter for
  forwarding services into I2P and proxying client requests to and from I2P. It
  provides a variety of "Tunnel Types" which are able able to do advance
  filtering of traffic before it reaches I2P.
 3. **[I2PSnark/Bittorrent](http://localhost:7657/torrents):** This is an I2P-Only bittorrent client, it never
  makes a connection to a peer over any other network,
 4. **[The Addressbook](http://localhost:7657/dns):** This is a simple, locally-defined list of
  human-readable addresses and corresponding I2P addresses. It integrates
  with other applications to allow the user to use those human-readable
  addresses in place of those I2P addresses.
 5. **[SusiMail/E-Mail](http://localhost:7657/webmail):** SusiMail is a secure e-mail client which is primarily
  intended for use with Postman's e-mail servers inside of I2P. It is designed
  to avoid leaking information about e-mail use to other networks, as many
  e-mail clients sometimes do.
 6. **[The QR Code Generator](http://localhost:7657/imagegen):** Besides the Addressbook, I2P addresses can be
  shared by converting them into QR codes and scanning them with a camera. This
  is especially useful for Android devices where typing is inconvenient.
- **Applications *Outside I2P* to use with I2P**
 1. **[Mozilla Firefox](https://mozilla.org):** A web browser with advanced privacy and security
  features, this is the best browser to adapt to your I2P use.
 2. **[Chromium](https://chromium.org):** A web browser developed by Google that is the Open-Source base
  of Google Chrome, this is sometimes used as an alternative to Firefox.
 3. **[BiglyBT](https://biglybt.com):** A Feature-Rich bittorrent client. By that I mean absolutely
  riddled with features, really cool features, including I2P support and the
  unique ability to "Bridge" regular torrents in-to I2P so people can download
  them anonymously.
 4. **[OpenSSH](https://www.openssh.com/):** OpenSSH is a popular program used by systems administrators to
  remotely administer a server, or to provide "Shell" accounts for users on the
  server.
 5. **[Git](https://git-scm.com)/[Gitlab](https://gitlab.com):** Git is a source-code control tool which is distributed, and
  often recommends a fork-first workflow. Hosting source code on I2P is an
  important activity, so Gitlab-specific  instructions are available for all to
  use.
 6. **[Debian](https://debian.org) and [Ubuntu](https://ubuntu.com) GNU/Linux:** It is possible to obtain packages for
  Debian and Ubuntu GNU/Linux over I2P using apt-transport-i2p and
  apt-transport-i2phhtp. In the future, a bittorrent-based transport may also
  be developed.
- **Applications for *Developers* to create new things**
 1. **[The SAM API Bridge](https://geti2p.net/en/docs/api/samv3):** The SAM API is a language-independent API for
  writing applications that are I2P-native by communicating with the local I2P
  router. It can provide Streaming-like capabilities, Anonymous Datagrams, or
  Repliable Datagrams.
 2. **[The BOB API Bridge](https://geti2p.net/en/docs/api/bob):** This is a deprecated technology, BOB users should
  migrate to SAM  if it is possible for them to do so.
 3. **[The I2CP API](https://geti2p.net/en/docs/protocol/i2cp):** Not strictly an application, this is how Java applications
  communicate with the I2P router to set up tunnels, generate and manage keys,
  and communicate with other peers on the network.
