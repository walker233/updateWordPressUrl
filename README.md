# updateWordPressUrl
Bash Scripts that update a WordPress URL, intended to be used with AWS development WordPress sites.
The following are intended to be placed in /usr/local/updateWordPressUrl/

Scripts included:

autoUpdateWpName - Intended to be called from Userdata when AWS EC2 image is started.
wpUpdateUrl - Init Script to add to system startup.
updateWpName - Manual change of URL.
wp-cli - Wrapper script for wp-cli.phar. Download wp-cli.phar at http://wp-cli.org/

All scripts require wp-cli.phar.

After downloading the scripts you must update certain variables.

autoUpdateWpName, update the following:
 INSTALL_DIR - Set to directory with your WordPress program installed.
 ie. INSTALL_DIR="/var/www/html" # is the default for Amazon Linux, Redhat, and Centos.
 CURL - Set to the directory
 
wpUpdateUrl, update the following:
 exec - set to the full path to the autoUpdateWpName file exists.
 ie. exec=/usr/local/updateWordPressUrl/autoUpdateWpName

updateWpName, update the following:
 INSTALL_DIR - Set to directory with your WordPress program installed.
 ie. INSTALL_DIR="/var/www/html" # is the default for Amazon Linux, Redhat, and  Centos.


