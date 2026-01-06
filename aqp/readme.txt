in moonraker.conf file add * in line 28

shh to your printer.

root
Creality2024

type:
vi /usr/share/moonraker/moonraker.conf

moonraker.conf should open. add * as below. you may need to press "insert" key to enable edit mode

[authorization]
force_logins: False
cors_domains:
  * ;add this to enable wildcard for local connections from web browser to printer
  *.local
  *.lan
  *://app.fluidd.xyz

once edited, press ESC and type :wq
in the left corrner ":wq" should show. press ENTER the file is saved.
restart printer, type reboot

website should now access the printer. no other changes are needed to printer or slicer. you can use newest firmware 1.1.0.60 and 7.0 slicer!
