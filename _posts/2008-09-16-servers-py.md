---
layout: post
title: servers.py
created: 1221579802
categories:
- !ruby/string:Sequel::SQL::Blob |-
  cHl0aG9u
- !ruby/string:Sequel::SQL::Blob |-
  aW5zYW5pdHk=
---
<pre>
#!/usr/bin/env python
# lut4rp - 20080814

import os

print 'Speek, O Human... '
choice = raw_input()
if choice == 'go' :
    os.system('sudo /etc/init.d/apache2 start')
    os.system('sudo /etc/init.d/mysql start')
if choice == 'no' :
    os.system('sudo /etc/init.d/apache2 stop')
    os.system('sudo /etc/init.d/mysql stop')
if choice == 're' :
    os.system('sudo /etc/init.d/apache2 restart')
    os.system('sudo /etc/init.d/mysql restart')

</pre>
