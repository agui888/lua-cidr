# lua-wheels
This pure-Lua module include a useful tool for some computes with cidr, and without installing other modules.


### Usage

    local cidr = require "cidr"

    local first_address, last_address = cidr.parse_cidr(ip_cidr)  // ip_cidr formats like 192.168.10.10/24

    local ip_num = cidr.ip_2_number(ip)  // get the ip to decimal.

    if ip_num >= first_address and ip_num <= last_address then   // judge if ip lies between the cidr.
        return true
    else
        return false
    end


### Other

    This module now supports only ipv4.
