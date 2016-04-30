Linux Server Configuration
==========================

IP Address: 52.36.10.250

SSH Port: 2200

URL to hosted web application: http://ec2-52-36-10-250.us-west-2.compute.amazonaws.com/

## Summary of Software Installed:
1. Updated and upgraded all existing packages
2. Installed finger package
3. Installed apache2 package
4. Installed libapache2-mod-wsgi package
5. Installed postgresql package
6. Installed git package
7. Installed python-pip package
8. Installed python's Flask-SQLAlchemy package
9. Installed python's SQLAlchemy-Utils package
10. Installed python's oauth2client package
11. Installed python's requests package

## Summary of Configuration Changes Made:
1. Created users grader and catalog
2. Enabled sudo (with password) permissions for users grader and catalog
3. Configured public key encryption for users grader and catalog
4. Forced key based authentication
5. Disabled root remote login
6. Changed the SSH port from 22 to 2200
7. Configured the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
8. Restarted ssh service to apply the changes
9. Configured local timezones to UTC
10. Installed and enabled apache and mod_wsgi
11. Installed and configured PostgreSQL
12. Cloned the Luxury Rides Catalog application files into the /var/www/luxury_rides_catalog/ directory
13. Created and configured the required .wsgi file to serve the Luxury Rides catalog application
    * Added a luxury_rides_catalog.wsgi file to the /var/www/luxury_rides_catalog/ directory
14. Created, configured and enabled a new virtual host for the Luxury Rides Catalog application
    * Added a luxury_rides_catalog.conf file to the /etc/apache2/sites-available/ directory
15. Restarted apache to apply the changes
