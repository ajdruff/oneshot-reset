#oneshot-reset
>A self-destructing password reset script for WordPress sites

This script will allow you to reset a WordPress installations's administrator password as long as you have access to the server's files. It does not require you to have access to the database.

Except for the 'self-destruction' feature, this is the same script that appears here: [Emergency Password Reset Script](https://codex.wordpress.org/User:MichaelH/Orphaned_Plugins_needing_Adoption/Emergency)

The `self destruction` feature was implemented using a simple  `ulink` function call which should normally cause it to destroy itself on a successful password reset.



##Warning

>**Do not leave this script on your server or someone else could use it to change your password.** The script may or may not delete itself depending on the server's configuration and file permissions. The **script will not delete itself if the password reset is not successful.**



##Keep in Mind:
* Requires you know the administrator username.
* It updates the administrator password and sends an email to the administrator's email address.


#How to Use



1. Place `oneshot-reset.php` in the root of your WordPress installation (the same directory that contains wp-config.php). 
2. Visit `http://example.com/oneshot-reset.php` (where `example.com` is the domain of your website.)
3. As instructed, enter the administrator username (usually admin) and the new password, then click the `Update Options` button. A message is displayed noting the changed password. An email is sent to the administrator with the changed password information.
4. Check that `oneshot-reset.php` is indeed deleted, and if not, delete it.


#Contributors

* Andrew Druffner <andrew@nomstock.com>
* [MichaelH](https://codex.wordpress.org/User:MichaelH/Orphaned_Plugins_needing_Adoption/Emergency) 
