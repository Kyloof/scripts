#!/bin/sh

pgrep -x discord > /dev/null || /snap/bin/discord &
sleep 0.5
pgrep -x spotify > /dev/null || /snap/bin/spotify &

bspc desktop 5 -f
bspc desktop main -f

# reload sxhkd because for some reason dmenu won't work unless I do this
sleep 0.5 && pkill -USR1 -x sxhkd

