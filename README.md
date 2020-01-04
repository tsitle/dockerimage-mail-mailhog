# Mailhog Docker Image for AARCH64, ARMv7l, X86 and X64

Provides Mailhog, which is a handy SMTP mail server useful for local
and team application development.  
You can use this image to send mail to a SMTP host
and Mailhog provides the SMTP server and web frontend.  
For more information on Mailhog please see Mailhog [Github Repository](https://github.com/mailhog/MailHog).

## Docker Container usage
See the related GitHub repository [https://github.com/tsitle/dockercontainer-mail-mailhog](https://github.com/tsitle/dockercontainer-mail-mailhog)

## Source of Mailhog binary packages
The binary packages were built using 
[https://github.com/tsitle/dockercontainer-app-go\_native\_compiler](https://github.com/tsitle/dockercontainer-app-go_native_compiler)  
and the build script `build-mailhog.sh` that the repository contains.

## Configuration
[Configure MailHog](CONFIG.md)  
Source: [https://github.com/mailhog/MailHog/blob/master/docs/CONFIG.md](https://github.com/mailhog/MailHog/blob/master/docs/CONFIG.md)
