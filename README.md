This is disigned to be an alternative starting set of options for new weechat
users that we hope will be more frendly and help with some common frustrations
with the current defaults. This set of configs is maintained by the OSU Linux
User Group.

This repo has an accompanying guide that can be found at the.internet

Install
-------

1. insure that there is no ~/.weechat directory (if there is you should back this up)
2. git clone user@link.place in your home dir
3. profit (ok, you might need to finish the guide first)

Changes of config files
-----------------------

###irc.conf

- Show nick changes when smart filter is on
smart_filter_nick = off

- This line would be generated with the local systeam user when making a blank config
nicks = "osulug"

###weechat.conf

- Make hostlist bar look better
hotlist_buffer_separator = " "
hotlist_count_min_msg = 1
hotlist_prefix = ""
hotlist_sort = group_number_asc

- Last seen line marker
read_marker_string = "-"
chat_read_marker = lightgreen

- Status bar theme
status_count_highlight = lightred
status_count_msg = blue
status_count_other = gray
status_count_private = lightred
status_data_highlight = lightred
status_data_other = yellow
status_data_private = red
status_more = red
status_name = lightgreen
status_number = lightgreen
status_time = yellow
status.color_bg = default
status.color_delim = magenta
status.color_fg = yellow
status.separator = on

- Added keys
meta-b = "/bar toggle buffers"
meta-f = "/filter toggle irc_smart"
meta-n = "/bar toggle nicklist"

- Added filters
irc_smart = on;*;irc_smart_filter;*

###Changes to the "buffers" script defaults

Included Plugins
----------------

autojoin.py
buffers.pl
colorize_nicks.py
iset.pl

Maintenance
-----------

As all good this on github we are always happy to see how the comunity can make
this repo better. Pull requestis will be reviewed by someone (hopefully) and
some group of people of which I will atempt to exert undue influence over will
deside if your change(S) makes for a better weechat exprance.

###To Do
- fix all the repo/guide links once they have a new home.
- The color scheme for the non-selected buffers in a merged buffer was left
  defult. I thik the defaults suck and make it unreadible but I use the other
  extream and just make it all look the same. I tried to find a happy median but
  could not.

Git Ignore
----------

This repo contains a .gitignore file to go along with it. The idea being that
this could be a leaving repo the people can make inplace pull requests and
pulls from. I dont know how practical this will be. Some files sucj as irc.conf
are inherently problematic has then contain both config options and
usernames/passwords. any thoughts on how to best achive this would be greatly
appreciated.

