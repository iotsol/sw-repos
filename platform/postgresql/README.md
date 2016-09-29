# RPM Files
	http://yum.postgresql.org/9.5/redhat/rhel-7-x86_64/repoview/
- postgresql-unit95-1.0-1.rhel7.x86_64.rpm
- pgadmin4-1.0-rc1_6.rhel7.x86_64.rpm
- postgresql95-9.5.4-2PGDG.rhel7.x86_64.rpm
- postgresql95-server-9.5.4-2PGDG.rhel7.x86_64.rpm
- pgadmin4-web-1.0-rc1_6.rhel7.noarch.rpm
- postgresql95-libs-9.5.4-2PGDG.rhel7.x86_64.rpm
- postgresql95-contrib-9.5.4-2PGDG.rhel7.x86_64.rpm
- postgresql-jdbc-9.4.1211-1.rhel7.noarch.rpm

# PostgreSQL Yum Repository
To use the yum repository, you must first install the repository RPM. To do this, download the correct RPM from the repository RPM listing, and install it with commands like:

On RHEL and its derivatives:
	yum install http://yum.postgresql.org/9.5/redhat/rhel-7-x86_64/pgdg-redhat95-9.5-2.noarch.rpm

Once this is done, you can proceed to install and update packages the same way as the ones included in the distribution.

For RHEL and its derivatives:
	yum install postgresql95-server postgresql95-contrib

(or yum groupinstall "PostgreSQL Database Server 9.6 PGDG")
	service postgresql-9.5 initdb
	chkconfig postgresql-9.5 on service postgresql-9.5 start

