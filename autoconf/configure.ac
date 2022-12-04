# Must init the autoconf setup
# The first parameter is project name
# second is version number
# third is bug report address
AC_INIT([hello], [0.1], [neo.chen@fastonetech.com])

# Safety checks in case user overwritten --srcdir
AC_CONFIG_SRCDIR([src/main.c])

# Store the auxiliary build tools (e.g., install-sh, config.sub, config.guess)
# in this dir (build-aux)
AC_CONFIG_AUX_DIR([build-aux])

# Init automake, and specify this program use relaxed structures.
# i.e. this program doesn't follow the gnu coding standards, and doesn't have
# ChangeLog, COPYING, AUTHORS, INSTALL, README etc. files.
AM_INIT_AUTOMAKE([-Wall -Werror foreign subdir-objects])

# Check for C compiler
AC_PROG_CC
# We can add more checks in this section

# Tells automake to create a Makefile
# See https://www.gnu.org/software/automake/manual/html_node/Requirements.html
# AC_CONFIG_FILES([Makefile src/Makefile])
AC_CONFIG_FILES([Makefile])

# Generate the output
AC_OUTPUT

# Printing regular message
AC_MSG_NOTICE([Greetings from Autoconf])

# Prints an error message and stops the configure script
# AC_MSG_ERROR([We have an error here!])

# abc="yes"
# def="no"
# AS_IF([test "X$abc" = "Xyes"],           # test condition
#     [AC_MSG_NOTICE([abc is yes])],       # then case
#     [test "X$def" = "Xyes"],             # else if
#     [AC_MSG_NOTICE([def is yes])],
#     [AC_MSG_ERROR([abc check failed])]   # else case
#     )
