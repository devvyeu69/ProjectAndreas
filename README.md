exec permissions.cfg
# you probably don't want to change these!
# only change them if you're using a server with multiple network interfaces
endpoint_add_tcp "0.0.0.0:30120"
endpoint_add_udp "0.0.0.0:30120"

ensure mapmanager
ensure chat
ensure spawnmanager
ensure sessionmanager
ensure fivem
ensure hardcap
ensure rconlog
ensure scoreboard
ensure playernames
sv_scriptHookAllowed 0
start vMenu




# change this
rcon_password changeme

sv_hostname "Project Andreas"

# nested configs!
#exec server_internal.cfg

# loading a server icon (96x96 PNG file)
#load_server_icon myLogo.png

# convars for use from script
set temp_convar "hey world!"

# disable announcing? clear out the master by uncommenting this
#sv_master1 "

# want to only allow players authenticated with a third-party provider like Steam?
#sv_authMaxVariance 1
#sv_authMinTrust 5

# add system admins
add_ace group.admin command allow # allow all commands
add_ace group.admin command.quit deny # but don't allow quit
add_principal identifier.steam:110000112345678 group.admin # add the admin to the group
set steam_webApiKey "0CCB1E0586338D8B9DED74F8181A1180"
add_principal identifie.steam:"0CCB1E0586338D8B9DED74F8181A1180"
add_principal identifier.steam:https:/steamcommunity.com/profiles/76561199023165399 group.admin 



# remove the # to hide player endpoints in external log output
#sv_endpointprivacy true

# server slots limit (must be between 1 and 31)
sv_maxclients 28

# license key for server (https://keymaster.fivem.net)
sv_licenseKey "0eqdzf0tj9e9xea1snp8bncme90p0oqe"
