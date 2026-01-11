AC_PREREQ(2.53)

AC_INIT([mate-themes], [3.22.26], [https://mate-desktop.org])

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

# Check GTK+ theme engines
PKG_CHECK_MODULES(THEME_ENGINE,
 [gtk+-2.0 >= 2.0.0 dnl
  gdk-pixbuf-2.0 >= 2.0.0 ])

AC_CONFIG_FILES([
Makefile
desktop-themes/Makefile
desktop-themes/BlackMATE/Makefile
desktop-themes/BlackMATE/apps/Makefile
desktop-themes/BlackMATE/gtk-2.0/Makefile
desktop-themes/BlackMATE/gtk-2.0/assets/Makefile
desktop-themes/BlackMATE/gtk-2.0/Styles/Makefile
desktop-themes/BlackMATE/gtk-3.0/Makefile
desktop-themes/BlackMATE/gtk-3.0/assets/Makefile
desktop-themes/BlackMATE/gtk-3.0/window-controls/Makefile
desktop-themes/BlackMATE/metacity-1/Makefile
desktop-themes/BlackMATE/cinnamon/Makefile
desktop-themes/BlackMATE/unity/Makefile
desktop-themes/BlueMenta/Makefile
desktop-themes/BlueMenta/cinnamon/Makefile
desktop-themes/BlueMenta/emerald/Makefile
desktop-themes/BlueMenta/gtk-2.0/Makefile
desktop-themes/BlueMenta/gtk-2.0/apps/Makefile
desktop-themes/BlueMenta/gtk-2.0/apps/Caja/Makefile
desktop-themes/BlueMenta/gtk-2.0/apps/Handles/Makefile
desktop-themes/BlueMenta/gtk-2.0/apps/Null/Makefile
desktop-themes/BlueMenta/gtk-2.0/apps/Others/Makefile
desktop-themes/BlueMenta/gtk-2.0/widgets/Makefile
desktop-themes/BlueMenta/gtk-2.0/widgets/Null/Makefile
desktop-themes/BlueMenta/gtk-2.0/widgets/Others/Makefile
desktop-themes/BlueMenta/gtk-2.0/widgets/Panel/Makefile
desktop-themes/BlueMenta/gtk-2.0/widgets/Scale/Makefile
desktop-themes/BlueMenta/gtk-3.0/Makefile
desktop-themes/BlueMenta/gtk-3.0/assets/Makefile
desktop-themes/BlueMenta/gtk-3.0/borders/Makefile
desktop-themes/BlueMenta/gtk-3.0/window-controls/Makefile
desktop-themes/BlueMenta/metacity-1/Makefile
desktop-themes/BlueMenta/unity/Makefile
desktop-themes/BlueMenta/xfwm4/Makefile
desktop-themes/BlueMenta-dark/Makefile
desktop-themes/BlueMenta-dark/cinnamon/Makefile
desktop-themes/BlueMenta-dark/emerald/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/apps/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/apps/Caja/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/apps/Handles/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/apps/Null/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/apps/Others/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/widgets/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/widgets/Null/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/widgets/Others/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/widgets/Panel/Makefile
desktop-themes/BlueMenta-dark/gtk-2.0/widgets/Scale/Makefile
desktop-themes/BlueMenta-dark/gtk-3.0/Makefile
desktop-themes/BlueMenta-dark/gtk-3.0/assets/Makefile
desktop-themes/BlueMenta-dark/gtk-3.0/borders/Makefile
desktop-themes/BlueMenta-dark/gtk-3.0/window-controls/Makefile
desktop-themes/BlueMenta-dark/metacity-1/Makefile
desktop-themes/BlueMenta-dark/unity/Makefile
desktop-themes/BlueMenta-dark/xfwm4/Makefile
desktop-themes/Blue-Submarine/Makefile
desktop-themes/Blue-Submarine/cinnamon/Makefile
desktop-themes/Blue-Submarine/emerald/Makefile
desktop-themes/Blue-Submarine/gtk-2.0/Makefile
desktop-themes/Blue-Submarine/gtk-2.0/apps/Makefile
desktop-themes/Blue-Submarine/gtk-2.0/apps/Handles/Makefile
desktop-themes/Blue-Submarine/gtk-2.0/apps/Panel/Makefile
desktop-themes/Blue-Submarine/gtk-2.0/assets/Makefile
desktop-themes/Blue-Submarine/gtk-3.0/Makefile
desktop-themes/Blue-Submarine/gtk-3.0/assets/Makefile
desktop-themes/Blue-Submarine/metacity-1/Makefile
desktop-themes/Green-Submarine/Makefile
desktop-themes/Green-Submarine/cinnamon/Makefile
desktop-themes/Green-Submarine/emerald/Makefile
desktop-themes/Green-Submarine/gtk-2.0/Makefile
desktop-themes/Green-Submarine/gtk-2.0/apps/Makefile
desktop-themes/Green-Submarine/gtk-2.0/apps/Handles/Makefile
desktop-themes/Green-Submarine/gtk-2.0/apps/Panel/Makefile
desktop-themes/Green-Submarine/gtk-2.0/assets/Makefile
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
