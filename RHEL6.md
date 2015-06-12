# Introduction #

Here is installer package for Red Hat Enterprise Linux 6 x86\_64

# Repos #
  1. http://mirror.smartmedia.net.id/epel/6/x86_64/
  1. http://elgis.argeo.org/repos/6/elgis/x86_64/
  1. http://ftp.scientificlinux.org/linux/scientific/6.0/x86_64/os/Packages/
  1. http://ftp5.gwdg.de/pub/opensuse/repositories/Application:/Geo/RHEL_6/x86_64/
  1. http://li.nux.ro/download/nux/dextop/el6/x86_64/


# Script #
```
#!/bin/bash
yum install gd

wget http://elgis.argeo.org/repos/6/elgis/x86_64/proj-epsg-4.8.0-3.el6.x86_64.rpm
rpm -ivh proj-epsg-4.8.0-3.el6.x86_64.rpm

wget http://elgis.argeo.org/repos/6/elgis/x86_64/proj-nad-4.8.0-3.el6.x86_64.rpm
rpm -ivh proj-nad-4.8.0-3.el6.x86_64.rpm

wget http://elgis.argeo.org/repos/6/elgis/x86_64/proj-4.8.0-3.el6.x86_64.rpm
rpm -ivh proj-4.8.0-3.el6.x86_64.rpm



wget http://elgis.argeo.org/repos/6/elgis/x86_64/geos-3.3.8-2.el6.x86_64.rpm
rpm -ivh geos-3.3.8-2.el6.x86_64.rpm

#dependencies gdal
wget http://ftp.scientificlinux.org/linux/scientific/6.0/x86_64/os/Packages/blas-3.2.1-4.el6.x86_64.rpm
rpm -ivh blas-3.2.1-4.el6.x86_64.rpm

wget http://mirror.smartmedia.net.id/epel/6/x86_64/armadillo-3.800.2-1.el6.x86_64.rpm
rpm -ivh armadillo-3.800.2-1.el6.x86_64.rpm

wget http://mirror.smartmedia.net.id/epel/6/x86_64/CharLS-1.0-1.el6.x86_64.rpm
rpm -ivh CharLS-1.0-1.el6.x86_64.rpm

wget http://mirror.smartmedia.net.id/epel/6/x86_64/cfitsio-3.240-3.el6.x86_64.rpm
rpm -ivh cfitsio-3.240-3.el6.x86_64.rpm

wget http://mirror.smartmedia.net.id/epel/6/x86_64/libdap-3.11.0-1.el6.x86_64.rpm
rpm -ivh libdap-3.11.0-1.el6.x86_64.rpm
wget http://ftp5.gwdg.de/pub/opensuse/repositories/Application:/Geo/RHEL_6/x86_64/libfreexl1-1.0.0e-1.1.x86_64.rpm
rpm -ivh libfreexl1-1.0.0e-1.1.x86_64.rpm
wget http://elgis.argeo.org/repos/6/elgis/x86_64/libgeotiff-1.4.0-1.el6.x86_64.rpm
rpm -ivh libgeotiff-1.4.0-1.el6.x86_64.rpm

wget http://mirror.smartmedia.net.id/epel/6/x86_64/libgta-1.0.2-2.el6.x86_64.rpm
rpm -ivh libgta-1.0.2-2.el6.x86_64.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/hdf5-1.8.5.patch1-7.el6.x86_64.rpm
rpm -ivh hdf5-1.8.5.patch1-7.el6.x86_64.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/netcdf-4.1.1-3.el6.5.x86_64.rpm
rpm -ivh netcdf-4.1.1-3.el6.5.x86_64.rpm
wget http://elgis.argeo.org/repos/6/elgis/x86_64/libspatialite-2.4.0-0.6_0.RC4.el6.x86_64.rpm
rpm -ivh libspatialite-2.4.0-0.6_0.RC4.el6.x86_64.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/xerces-c-3.0.1-0.20.1.el6.x86_64.rpm
rpm -ivh xerces-c-3.0.1-0.20.1.el6.x86_64.rpm





#dependensi gpsbabel
wget http://elgis.argeo.org/repos/6/elgis/x86_64/gdal-libs-1.9.2-4.el6.x86_64.rpm
rpm -ivh gdal-libs-1.9.2-4.el6.x86_64.rpm

wget http://mirror.smartmedia.net.id/epel/6/x86_64/shapelib-1.2.10-21.20060304cvs.x86_64.rpm
rpm -ivh shapelib-1.2.10-21.20060304cvs.x86_64.rpm
#gpsbabel butuh dependensi
wget http://elgis.argeo.org/repos/6/elgis/x86_64/gpsbabel-1.4.4-1.el6.x86_64.rpm
rpm -ivh gpsbabel-1.4.4-1.el6.x86_64.rpm


wget http://elgis.argeo.org/repos/6/elgis/x86_64/gdal-1.9.2-4.el6.x86_64.rpm
rpm -ivh gdal-1.9.2-4.el6.x86_64.rpm

yum install curl


wget http://elgis.argeo.org/repos/6/elgis/x86_64/postgis-1.5.8-1.el6.x86_64.rpm
rpm -ivh postgis-1.5.8-1.el6.x86_64.rpm

#dependensi mapserver
wget http://li.nux.ro/download/nux/dextop/el6/x86_64/bitstream-vera-fonts-common-1.10-19.el6.nux.noarch.rpm
rpm -ivh bitstream-vera-fonts-common-1.10-19.el6.nux.noarch.rpm

wget http://li.nux.ro/download/nux/dextop/el6/x86_64/bitstream-vera-sans-fonts-1.10-19.el6.nux.noarch.rpm
rpm -ivh bitstream-vera-sans-fonts-1.10-19.el6.nux.noarch.rpm


wget http://mirror.smartmedia.net.id/epel/6/x86_64/fcgi-2.4.0-10.el6.x86_64.rpm
rpm -ivh fcgi-2.4.0-10.el6.x86_64.rpm

wget http://li.nux.ro/download/nux/dextop/el6/x86_64/libfribidi-0.19.2-3.el6.nux.x86_64.rpm
rpm -ivh libfribidi-0.19.2-3.el6.nux.x86_64.rpm

#mapserver butuh dependensi
wget http://elgis.argeo.org/repos/6/elgis/x86_64/mapserver-6.0.3-4_0.el6.x86_64.rpm
rpm -ivh mapserver-6.0.3-4_0.el6.x86_64.rpm


ln -s /usr/sbin/mapserv /var/www/cgi-bin/mapserv
```

Edit file :
/etc/httpd/conf/httpd.conf
in the block of cgi directories, change the setting like this :
```
ScriptAlias /cgi-bin/ "/var/www/cgi-bin/"

#
# "/var/www/cgi-bin" should be changed to whatever your ScriptAliased
# CGI directory exists, if you have that configured.
#
<Directory "/var/www/cgi-bin">
    AllowOverride All
    Options +Indexes +ExecCGI
	Order allow,deny
    Allow from all
</Directory>
```