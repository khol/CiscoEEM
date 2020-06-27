# CiscoEEM
Cisco Embedded Event Manager scripts

the scripts is for update description when somthing hapends to the switch port.
if a dot1x client or a switch we handle that diffrent

the: auto_1x_access_port_inter_description_update.txt adds data to the variables below and than apply it to the interface descriptoon. 
"Access:$TODAYSDATE: - $MACTOVLAN - $DOT1XUSER - $DOT1XIP - $USERMACADDR - $DOT1XAUTH "

the: auto_cdp-lldp_interface_description_update.txt adds data to description from cdp/lldp information on the interface
"Access:$TODAYSDATE - $acc_port - $int" or "Trunk:$TODAYSDATE - $int"

the: fix_date_to_interface_description_update.txt get the data on the format $YEAR$MONTH$DAY, to use this in the other scripts, than vi put the date in a file in flash:
