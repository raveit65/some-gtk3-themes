AC_PREREQ(2.53)

AC_INIT([some-gtk3-themes], [1.0.0], [https://github.com/raveit65/some-gtk3-themes])

AM_INIT_AUTOMAKE([1.9 tar-ustar dist-xz no-dist-gzip check-news])

# Enable silent build rules by default, requires at least
# Automake-1.11. Disable by either passing --disable-silent-rules to
# configure or passing V=1 to make
m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

AM_GNU_GETTEXT([external])
PKG_PROG_PKG_CONFIG([0.19])
AM_GNU_GETTEXT_VERSION([0.19.8])
AM_CONDITIONAL([USE_NLS], [test "x${USE_NLS}" = "xyes"])

# Workaround to make aclocal get the right flags
AC_SUBST(ACLOCAL_AMFLAGS, "\${ACLOCAL_FLAGS}")

AC_CONFIG_FILES([
Makefile
desktop-themes/Makefile
desktop-themes/BlackMATE/Makefile
desktop-themes/BlackMATE/apps/Makefile
desktop-themes/BlackMATE/gtk-3.0/Makefile
desktop-themes/BlackMATE/gtk-3.0/assets/Makefile
desktop-themes/BlackMATE/gtk-3.0/window-controls/Makefile
desktop-themes/BlackMATE/metacity-1/Makefile
desktop-themes/BlackMATE/cinnamon/Makefile
desktop-themes/BlackMATE/unity/Makefile
desktop-themes/BlueMenta/Makefile
desktop-themes/BlueMenta/cinnamon/Makefile
desktop-themes/BlueMenta/emerald/Makefile
desktop-themes/BlueMenta/gtk-3.0/Makefile
desktop-themes/BlueMenta/gtk-3.0/assets/Makefile
desktop-themes/BlueMenta/gtk-3.0/borders/Makefile
desktop-themes/BlueMenta/gtk-3.0/window-controls/Makefile
desktop-themes/BlueMenta/metacity-1/Makefile
desktop-themes/BlueMenta/unity/Makefile
desktop-themes/BlueMenta/xfwm4/Makefile
desktop-themes/DarkMenta/Makefile
desktop-themes/DarkMenta/cinnamon/Makefile
desktop-themes/DarkMenta/emerald/Makefile
desktop-themes/DarkMenta/gtk-3.0/Makefile
desktop-themes/DarkMenta/gtk-3.0/assets/Makefile
desktop-themes/DarkMenta/gtk-3.0/borders/Makefile
desktop-themes/DarkMenta/gtk-3.0/window-controls/Makefile
desktop-themes/DarkMenta/metacity-1/Makefile
desktop-themes/DarkMenta/unity/Makefile
desktop-themes/DarkMenta/xfwm4/Makefile
desktop-themes/Blue-Submarine/Makefile
desktop-themes/Blue-Submarine/cinnamon/Makefile
desktop-themes/Blue-Submarine/emerald/Makefile
desktop-themes/Blue-Submarine/gtk-3.0/Makefile
desktop-themes/Blue-Submarine/gtk-3.0/assets/Makefile
desktop-themes/Blue-Submarine/metacity-1/Makefile
desktop-themes/Green-Submarine/Makefile
desktop-themes/Green-Submarine/cinnamon/Makefile
desktop-themes/Green-Submarine/emerald/Makefile
desktop-themes/Green-Submarine/gtk-3.0/Makefile
desktop-themes/Green-Submarine/gtk-3.0/assets/Makefile
desktop-themes/Green-Submarine/metacity-1/Makefile
po/Makefile.in
])

AC_OUTPUT

dnl ==========================================================================
echo "
Configure summary:

    ${PACKAGE_STRING}
    `echo $PACKAGE_STRING | sed "s/./=/g"`

    Installation prefix ........: ${prefix}
    Native Language support ....: ${USE_NLS}
"
