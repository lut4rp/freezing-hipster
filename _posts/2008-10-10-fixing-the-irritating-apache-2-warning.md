---
layout: post
title: Fixing the irritating Apache 2 warning
created: 1223616315
categories:
- !ruby/string:Sequel::SQL::Blob |-
  bGludXg=
- !ruby/string:Sequel::SQL::Blob |-
  YXBhY2hl
---
For all those who have been using Apache 2 on a localhost on a Linux distro, there's this weird (and very irritating) warning that one gets whenever the Apache server is started or stopped.
<em>Could not reliably determine the server's fully qualified domain name, using 127.0.1.1 for ServerName</em>

The address you get here might vary, but the error persists. Here's how to fix it -

* Open /etc/apache2/apache2.conf in your favourite text editor.
* Find the line that says <code>ServerRoot "/etc/apache2"</code>
* Add another line below it <code>ServerName "localhost"</code>
* Restart Apache server.
* Heave a sigh of relief from that darn irritant.

NOTE: This is valid only if you are running Apache on a localhost. If you're running it for a different domain, you'll probably need to replace localhost with your host name.
<!--break-->
