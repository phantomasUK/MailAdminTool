MailAdminTool
=============

Mail Admin Tool based on work by Steffan Slot from http://mat.ssdata.dk/ with improvemnets by Tarek Loubani.
This is a version with improved password security.

This management interface is for the purpose of administering email servers, originally created and distributed by Stefan Slot (mat@ssdata.dk).
It is made with the ISPmail guide (http://workaround.org/ispmail) in mind, and with one exception it works with the database created when following that guide.
IMPORTANT! In the virtual_users table the password column type needs to be varchar(106) not varchar(32) because of the
stronger password hashing.
Ref. (https://www.linode.com/docs/email/postfix/email-with-postfix-dovecot-and-mysql)

## Requirements
* A webserver with PHP support
* Javascript
* Access to the mysql server containing the "Mailserver" database from the webserver

## Setup
Database settings are found in the `includes/config.php`


Even if this tool has password access, you should only allow your own IP or local IP range to access the page with a .htaccess file on your webserver!

Per Steffan Slot's original notice:
"You can make changes, give it to others, whatever you want with it, but I do require that you always leave the footer like it is at the bottom saying 'This tool was made by Steffan Slot (http://mat.ssdata.dk)'"

His original changelog and README.txt are provided as requested in his notice.
