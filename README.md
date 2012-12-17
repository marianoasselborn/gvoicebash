gvoicebash
==========

Bash script to send sms messages from the command line.

Useful when in need of a programatic way to send quick results of alerts via sms. Requires a
Google account that already has access to Voice with a number assigned.

This is a work in progress!!


Usage:
======
./gvoicebash -u yourgoogleaccount@gmail.com -p yourgooglepassword -n destinationnumber -m "Your message between double quotes"

You should get a "Message sent successfully" as a return. If something is wrong, you'll get an ERROR message.

Tip: Throw the location of the script in your PATH variable if you want to call it from any location, or create a symlink under /bin


Next steps:
===========
- Changing the way the script takes the password so it's not necessary to pass it as an argument (use a password prompt instead).
- Make the script be able to read a user config file located under /home/user so the script can be called automatically without having to leave the password visible (ex. when using cron).
- Test for getopts values and exit if something funky is entered. Right now this is very loose.

If you have some ideas, open an issue to share them!