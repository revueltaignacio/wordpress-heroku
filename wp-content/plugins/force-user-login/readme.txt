=== Force User Login ===
Contributors: Integer Development
Donate Link: Don't worry about it
Tags: force user login, login, password, privacy
Requires at least: 2.0.2
Tested up to: 2.1
Stable tag: 1.2

Very small plugin that forces users to login to view blog content.

== Description ==

This is a very small plugin that forces users to login before viewing any content. This is done by checking if the user is logged in, and if not, redirecting them to the login page. Users attempting to view blog content via RSS are also authenticated via HTTP Auth. 

== Installation ==

1. Upload `force-login.php` to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==

= Can I change where the user is redirected after logging in? =

Yes! A variable called $redirect_to (line 33) is currently set to redirect the user to the page they were trying to access. If you changed that line from

`$redirect_to = $_SERVER['REQUEST_URI'];`

to

`$redirect_to = '/';`

it would redirect the user to the home page.

== Screenshots ==

None taken.. Just a login screen.