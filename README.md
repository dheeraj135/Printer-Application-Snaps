# Printer-Application-Snaps

This is snap for hplip printer driver package.

# How to install:
From the snap store:
```
snap install --edge hplip-printer-application
snap connect hplip-printer-application:avahi-control
snap connect hplip-printer-application:raw-usb
snap connect hplip-printer-application:hardware-observe
snap restart hplip-printer-application
```
Using the snapcraft.yaml file:
```
snapcraft
snap install hplip-printer-application_VERSION_ARCH.snap
snap connect hplip-printer-application:avahi-control
snap connect hplip-printer-application:raw-usb
snap connect hplip-printer-application:hardware-observe
snap restart hplip-printer-application
```
