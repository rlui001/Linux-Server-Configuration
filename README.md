# Linux-Server-Configuration

- IP Address: 54.173.188.9
- Port: 2200
- URL: ec2-54-173-188-9.compute-1.amazonaws.com
- NO LONGER WORKING; SHUT DOWN

# To update server
- sudo apt-get update
- sudo apt-get upgrade

# Software installed to run flask application
- postgresql
- psycopg2
- flask
- requests
- oauth2client
- sqlalchemy
- pip
- virtualenv (although not used)
- git
- mod_wsgi
- apache2

# Configuration changes made
- Changed SSH port from 22 to 2200
- Added user 'grader' with sudo rights in sudoers.d directory
- Changed timezone to UTC
- Added rules to ufw and enabled
- Added incoming port on Amazon Lightsail (to enable SSH via custom 2200 port)
- Updated public SSH key on server so 'grader' can SSH



# Third-party resources 
- stackoverflow.com - Troubleshooting tasks such as import errors, linux commands, git cloning
- askubuntu.com - Setting timezone, problems with fetching archives(apt-get update errors)
- linode.com - Setting up apache and modwsgi on Ubuntu, configurations
- jakowicz.com - More information on setting up an apache web server that runs flask applications, wsgi configurations
- hcidata.info - Used to convert IP Address to host name/url
- dabapps.com - Pip and virtualenv information, installation guide
- postgresql.org / tutorialspoint.com - Tutorials and documentation on setting up postgresql, database, user/permissions
