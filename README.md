Passwordless
============

This module replaces the regular Drupal login form with a modification of the password-
request form, to give the possibility to log in without using a password.

Every time a user needs to log in, only the e-mail address is required. The login link 
will be sent to the user's e-mail address, and will expire in 24 hours if not used.

Passwordless disables the password-reset form, and changes the relevant settings at 
admin/config/people/accounts. Uninstalling the module will restore everything to the way 
it was before (including the settings).

Note
----

Passwordless disables the password fields in user-registration and user-profile forms, 
which means that:

1. The system takes care of creating a password for new users.
2. There's no longer a requirement for users to reenter their current password when they 
enter a new e-mail address in their profile.

Due to point number 2, Passwordless depends on 
[Email Change Confirmation](http://drupal.org/project/email_confirm), 
unless <https://github.com/backdrop/backdrop-issues/issues/5210> is resolved. 
Make sure you save settings at `admin/config/people/email_confirm`, including the "From" 
address, for the module to work properly.

Settings
--------

Passwordless settings can be found at `admin/config/system/passwordless`.

Current Maintainers
-------------------

- [Herb v/d Dool](https://github.com/herbdool/)
- Seeking co-maintainers.

Credits
-------

Ported to Backdrop by [Herb v/d Dool](https://github.com/herbdool/).

Originally developed for Drupal by [greggles](https://www.drupal.org/u/greggles), [jaydub](https://www.drupal.org/u/jaydub).

Passwordless follows the idea behind [NoPassword](https://nopassword.alexsmolen.com), but 
is all based on Drupal's native functionality and code.

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.
