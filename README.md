# Linux-Server-Configuration

IP Address: 52.36.10.250

SSH Port: 2200

URL to hosted web application: http://ec2-52-36-10-250.us-west-2.compute.amazonaws.com/

## Summary of Software Installed:
Updated and upgraded all existing packages
Installed finger package
Installed apache2 package
Installed libapache2-mod-wsgi package
Installed postgresql package
Installed git package
Installed python-pip package
Installed python's Flask-SQLAlchemy package
Installed python's SQLAlchemy-Utils package
Installed python's oauth2client package
Installed python's requests package

## Summary of Configuration Changes Made:
Created users grader and catalog
Enabled sudo (with password) permissions for users grader and catalog
Configured public key encryption for users grader and catalog
Forced key based authentication
Disabled root remote login
Restarted ssh service to apply the changes
Configured local timezones to UTC
Installed and enabled apache and mod_wsgi
Cloned the Luxury Rides Catalog application files into the /var/www/luxury_rides_catalog directory
Created and configured the required .wsgi file to serve the Luxury Rides catalog application
Added a luxury_rides_catalog.wsgi file to the /var/www/luxury_rides_catalog/ directory
Created, configured and enabled a new virtual host for the Luxury Rides Catalog application
Added a luxury_rides_catalog.conf file to the /etc/apache2/sites-available/ directory
Restarted apache to apply the changes
