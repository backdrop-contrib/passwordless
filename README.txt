This module replaces the regular Drupal login form with a modification of the password-request form, to give the possibility to log in without using a password.

Every time a user needs to log in, only the e-mail address is required. The login link will be sent to the user's e-mail address, and will expire in 24 hours if not used.

Passwordless follows the idea behind [NoPassword](https://nopassword.alexsmolen.com), but is all based on Drupal's native functionality.

### Disclaimer
This is still an experimental module, and using it on production sites is not recommended.