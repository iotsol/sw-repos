# RPM Files
	http://yum.postgresql.org/9.5/redhat/rhel-7-x86_64/repoview/

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

