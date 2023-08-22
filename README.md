Foreman Katello plugin SELinux poclicy
======================================

SELinux policies for Foreman Katello plugin

Compiling
---------

To locally compile the policy do something like:

    PCY=katello
    sed -i s/@@VERSION@@/99.9/ $PCY.te
    make -f /usr/share/selinux/devel/Makefile load NAME=$PCY

There's a target to do this on remote system via ssh:

    make remote-load HOST=my.host.lan

License
-------

Copyright (c) 2015 Red Hat, Inc.

This program and entire repository is free software: you can redistribute it
and/or modify it under the terms of the GNU General Public License as
published by the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see <http://www.gnu.org/licenses/>.

