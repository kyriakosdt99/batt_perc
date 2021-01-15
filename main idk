#!/usr/bin/bash

#Current battery capacity
_current=$( < /sys/class/power_supply/BAT0/capacity )

#Display wether the battery is charging or discharching
#_status=$( < /sys/class/power_supply/BAT0/status )

if [[ $_current -ge 85 ]]; then
        echo -e "[$_status \uf240  $_current %]";
        exit;
fi
if [[ $_current -ge 60 ]]; then
        echo -e "[$_status \uf241  $_current %]";
        exit;
fi
if [[ $_current -ge 35 ]]; then
        echo -e "[$_status \uf242  $_current %]";
        exit;
fi
if [[ $_current -ge 10 ]]; then
        echo -e "[$_status \uf243  $_current %]";
        exit;
fi
#Default
echo -e "[$_status \uf244  $_current %]"
