# batocera-custom-es_systems
EmulationStation displays systems based on a file called es_systems.cfg. In other distributions, this is typically the only file. However, in Batocera FIXME and higher, the /userdata/system/configs/emulationstation/es_systems_&lt;custom_name>.cfg can be used as an overlay to the original /usr/share/emulationstation/es_systems.cfg file.

You must use a unique <name> field when adding a new system if you wish to keep the old one in addition. However, if using duplicate shortnames is a necessity and you still want the new and old system to exist simultaneously, you can also put both systems in a single CFG file.
