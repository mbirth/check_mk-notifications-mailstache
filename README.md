Mailstache for Check_MK
=======================

Unpack everything to your OMD site's "local" directory so that the final structure is like this:

```
.../sites/YOURSITE
           `-local
               |-lib
               |   |-external
               |   |   `-pystache (dir)
               |   `-python
               |       `-pystache (Symlink)
               `-share
                   `-check_mk
                       `-notifications
                           |-mailstache_templates
                           |   |-foot_html.mustache
                           |   |-head_html.mustache
                           |   |-host_html.mustache
                           |   |-host_subject.mustache
                           |   |-host_txt.mustache
                           |   |-service_html.mustache
                           |   |-service.subject.mustache
                           |   `-service_txt.mustache
                           `-mailstache (executable)
```

If you are using Check_MK without OMD, the directories may differ. You may also have to modify the `mailstache` script accordingly.
