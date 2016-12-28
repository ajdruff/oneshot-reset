
#Self Destructing WordPress Password Reset



This is the same script that appears here:

[Emergency Password Reset Script](https://codex.wordpress.org/User:MichaelH/Orphaned_Plugins_needing_Adoption/Emergency)

except that it has a `ulink` function call which should normally cause it to destroy itself on a successful password reset.


you wouldn't need the script.

##Warning

* The script may or may not delete itself depending on the server's configuration and file permissions.
* Do not leave this script on your server or you risk your site being easily hacked.


##Keep in Mind:
* Requires you know the administrator username.
* It updates the administrator password and sends an email to the administrator's email address.
* You do not need to be logged in to WordPress to use it. 


#How to Use



1. Place this in the root of your WordPress installation (the same directory that contains wp-config.php). 
2. Go to http://example.com/password-reset.php where example.com is the domain of your website.
3. As instructed, enter the administrator username (usually admin) and the new password, then click Update Options. A message is displayed noting the changed password. An email is sent to the blog administrator with the changed password information.
4. Check that password-reset.php is indeed deleted, and if not, delete it.

**Do not leave this script on your server or someone else could use it to change your password.
**
