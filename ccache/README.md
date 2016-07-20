# Andrew's ccache spec file

Current [ccache](https://ccache.samba.org/) for CentOS 7 and similar distros.

## Prerequistes
- rpm-build `sudo yum install rpm-build`
- This ccache.spec file
- The existing EPEL [ccache.srpm file](https://dl.fedoraproject.org/pub/epel/7/SRPMS/c/ccache-3.1.9-3.el7.src.rpm)

## Build/Install current ccache with this ccache.spec file
- Install the above EPEL ccache.srpm file
- Place the new included ccache.spec file in rpmbuild/SPEC
- Build the new ccache with `rpmbuild -bb ccache.spec`
- Install with `sudo yum localinstall rpmbuild/RPMS/ccache-3*`
