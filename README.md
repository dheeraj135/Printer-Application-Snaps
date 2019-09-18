# Printer-Application-Snaps

## Gutenprint

Using the snapcraft.yaml file:
```
./configure --disable-pwgonly
snapcraft
snap install gutenprint-printer-application_VERSION_ARCH.snap
snap connect gutenprint-printer-application:avahi-control
snap connect gutenprint-printer-application:raw-usb
snap connect gutenprint-printer-application:hardware-observe
snap restart gutenprint-printer-application
```