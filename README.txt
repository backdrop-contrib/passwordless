This module replaces the regular Drupal login form with a modification of the password-request form, to give the possibility to log in without using a password.

Every time a user needs to log in, only the e-mail address is required. The login link will be sent to the user's e-mail address, and will expire in 24 hours if not used.

Passwordless disables the password-reset form, and changes the relevant settings at admin/config/people/accounts. Uninstalling the module will restore everything to the way it was before (including the settings). It's also compatible with other login-enhancing modules, like [LoginToboggan](http://drupal.org/project/logintoboggan).

### Due credit

Passwordless follows the idea behind [NoPassword](https://nopassword.alexsmolen.com), but is all based on Drupal's native functionality and code.

### Disclaimer
This is still an experimental module, and using it on production sites is not recommended.