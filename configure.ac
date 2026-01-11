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
desktop-themes/BlackMATE-border/Makefile
desktop-themes/BlackMATE-border/metacity-1/Makefile
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
desktop-themes/BlueMenta-border/Makefile
desktop-themes/BlueMenta-border/metacity-1/Makefile
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
desktop-themes/Blue-Submarine-border/Makefile
desktop-themes/Blue-Submarine-border/metacity-1/Makefile
desktop-themes/ContrastHigh/Makefile
desktop-themes/GreenLaguna/Makefile
desktop-themes/GreenLaguna/gtk-2.0/Makefile
desktop-themes/GreenLaguna/gtk-2.0/Styles/Makefile
desktop-themes/GreenLaguna/gtk-3.0/Makefile
desktop-themes/GreenLaguna/gtk-3.0/assets/Makefile
desktop-themes/GreenLaguna/gtk-3.0/window-controls/Makefile
desktop-themes/GreenLaguna/metacity-1/Makefile
desktop-themes/GreenLaguna/unity/Makefile
desktop-themes/GreenLaguna-border/Makefile
desktop-themes/GreenLaguna-border/metacity-1/Makefile
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
desktop-themes/Green-Submarine-border/Makefile
desktop-themes/Green-Submarine-border/metacity-1/Makefile
desktop-themes/HighContrastInverse/Makefile
desktop-themes/HighContrastInverse/gtk-2.0/Makefile
desktop-themes/HighContrastInverse/gtk-2.0/gtkrc
desktop-themes/HighContrastInverse/metacity-1/Makefile
desktop-themes/HighContrastInverse/pixmaps/Makefile
desktop-themes/Menta/Makefile
desktop-themes/Menta/cinnamon/Makefile
desktop-themes/Menta/emerald/Makefile
desktop-themes/Menta/gtk-2.0/Makefile
desktop-themes/Menta/gtk-2.0/apps/Makefile
desktop-themes/Menta/gtk-2.0/apps/Caja/Makefile
desktop-themes/Menta/gtk-2.0/apps/Handles/Makefile
desktop-themes/Menta/gtk-2.0/apps/Null/Makefile
desktop-themes/Menta/gtk-2.0/apps/Others/Makefile
desktop-themes/Menta/gtk-2.0/widgets/Makefile
desktop-themes/Menta/gtk-2.0/widgets/Null/Makefile
desktop-themes/Menta/gtk-2.0/widgets/Others/Makefile
desktop-themes/Menta/gtk-2.0/widgets/Panel/Makefile
desktop-themes/Menta/gtk-2.0/widgets/Scale/Makefile
desktop-themes/Menta/gtk-3.0/Makefile
desktop-themes/Menta/gtk-3.0/assets/Makefile
desktop-themes/Menta/gtk-3.0/borders/Makefile
desktop-themes/Menta/gtk-3.0/window-controls/Makefile
desktop-themes/Menta/metacity-1/Makefile
desktop-themes/Menta/unity/Makefile
desktop-themes/Menta/xfwm4/Makefile
desktop-themes/Menta-border/Makefile
desktop-themes/Menta-border/metacity-1/Makefile
desktop-themes/TraditionalGreen/Makefile
desktop-themes/TraditionalGreen/gtk-2.0/Makefile
desktop-themes/TraditionalGreen/gtk-3.0/Makefile
desktop-themes/TraditionalGreen/gtk-3.0/img/Makefile
desktop-themes/TraditionalGreen/metacity-1/Makefile
desktop-themes/TraditionalOk/Makefile
desktop-themes/TraditionalOk/gtk-2.0/Makefile
desktop-themes/TraditionalOk/gtk-3.0/Makefile
desktop-themes/TraditionalOk/gtk-3.0/img/Makefile
desktop-themes/TraditionalOk/metacity-1/Makefile
desktop-themes/TraditionalOk/openbox-3/Makefile
desktop-themes/TraditionalOk/xfwm4/Makefile
desktop-themes/TraditionalOk/xfwm4/png/Makefile
desktop-themes/YaruOk/Makefile
desktop-themes/YaruOk/gtk-2.0/Makefile
desktop-themes/YaruOk/gtk-3.0/Makefile
desktop-themes/YaruOk/gtk-3.0/assets/Makefile
desktop-themes/YaruOk/metacity-1/Makefile
desktop-themes/YaruOk/openbox-3/Makefile
desktop-themes/YaruOk/xfwm4/Makefile
desktop-themes/YaruOk/xfwm4/png/Makefile
desktop-themes/YaruGreen/Makefile
desktop-themes/YaruGreen/gtk-2.0/Makefile
desktop-themes/YaruGreen/gtk-3.0/Makefile
desktop-themes/YaruGreen/gtk-3.0/assets/Makefile
desktop-themes/YaruGreen/metacity-1/Makefile
marco-themes/Makefile
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
