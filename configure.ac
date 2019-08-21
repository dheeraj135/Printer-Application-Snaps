# PACKAGE=Printer-Application-Snaps
# VERSION=0.0.1

AC_INIT([Printer-Application-Snaps],[0.0.1],[])

AC_CONFIG_FILES(snap/local/snapcraft.yaml,[mv snap/local/snapcraft.yaml snap/snapcraft.yaml])
# AC_CONFIG_FILES([build],[chmod u+x build])

pwgpatch=""
AC_ARG_ENABLE([pwgconv],[  --disable-pwgconv    Remove pwg-raster to cups-raster conv.],
[case "${enableval}" in
    yes) pwgpatch="";;
    no) pwgpatch="#";;
    *) AC_MSG_ERROR([bad value ${enableval} for --disable-pwgconv]);;esac],[patch=""])

ippbranch="master"
AC_ARG_ENABLE([pwgonly],[  --disable-pwgonly    Accept other file formats along with pwg-raster.],
[case "${enableval}" in
    yes) ippbranch="master";;
    no) ippbranch="all_docformats";;
    *) AC_MSG_ERROR([bad value ${enableval} for --disable-pwgonly]);;esac])

AC_SUBST([pwgpatch])
AC_SUBST([ippbranch])

AC_OUTPUT