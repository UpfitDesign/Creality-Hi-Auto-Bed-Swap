in moonraker.conf file add * in line 28

[authorization]
force_logins: False
cors_domains:
  * ;add this to enable wildcard for local connections from web browser to printer
  *.local
  *.lan
  *://app.fluidd.xyz

