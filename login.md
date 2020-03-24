# Logging In

Logging in to your site is a straightforward process, and can additionally be secured with two-factor authentication.


## Logging in with Username/Password

To log in with username and password, just visit /user/login on your site. For example, if your site is https://www.mysite.com, 
you would visit https://www.mysite.com/user/login

Enter your email address and password, and optionally have the site "remember" your login so that you remain logged in until
you manually log out. 

<div style="background: #ffcccb; padding: 1em; border-radius: 1em; text-align: center; font-weight: bold;">
Note: Do not enable "remember me" on public systems, or systems that you share with others.
</div>

## Logging in with Two Factor Auth

If you, or your system administrator, has enabled two-factor authentication for your account, you will be asked to enter
a six digit code (one time password) after authenticating with your email address and password. 

There are many tools available to manage two-factor authentication, including:

* Google Authenticator ([iPhone](https://apps.apple.com/in/app/google-authenticator/id388497605), [Android)](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_IN)
* Microsoft Authenticator ([iPhone](https://apps.apple.com/us/app/microsoft-authenticator/id983156458), [Android](https://play.google.com/store/apps/details?id=com.azure.authenticator&hl=en_IN))
* Authy ([iPhone](https://apps.apple.com/in/app/authy/id494168017), [Android](https://play.google.com/store/apps/details?id=com.authy.authy&hl=en_IN))

In addition, many password management applicatons, such as 1Password and BitWarden offer support for two-factor authentication.

## Social Media Accounts

If your system administrator has enabled logging in through social media, then you can log in by clicking on the appropriate button
on the login page. Currently support social media logins are limited to:

* Google
* Facebook
* GitHub