# Notice

This is a Community-supported project.

If you are interested in becoming a maintainer of this project, please contact us at integrations@globee.com. Developers at GloBee will attempt to work with new maintainers to ensure the project remains viable for the foreseeable future.

# GloBee plugin for ECWID

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://raw.githubusercontent.com/GloBee-Official/ecwid-plugin/master/LICENSE.txt)

# Description

Bitcoin payment plugin for Ecwid using the globee.com service.


## Quick Start Guide

* Last Version Tested: 13.0.1629

To get up and running with our plugin quickly, see the GUIDE here: https://github.com/GloBee-Official/ecwid-plugin/blob/master/GUIDE.md


## Troubleshooting

The official GloBee API documentation should always be your first reference for development.

- Verify that your "notificationURL" for the invoice is "https://" (not "http://")
- Ensure a valid SSL certificate is installed on your server. Also ensure your root CA cert is updated. If your CA cert is not current, you will see curl SSL verification errors.
- Verify that your callback handler at the "notificationURL" is properly receiving POSTs. You can verify this by POSTing your own messages to the server from a tool like Chrome Postman.
- Verify that the POST data received is properly parsed and that the logic that updates the order status on the merchants web server is correct.
- Verify that the merchants web server is not blocking POSTs from servers it may not recognize. Double check this on the firewall as well, if one is being used.
- Use the logging functionality to log errors during development. If you contact BitPay support, they will ask to see the log file to help diagnose any problems.
- Check the version of this plugin against the official repository to ensure you are using the latest version. Your issue might have been addressed in a newer version of the library.

## Support
 
**GloBee Support:**

* [GitHub Issues](https://github.com/GloBee-Official/ecwid-plugin/issues)
  * Open an issue if you are having issues with this plugin.
* [Support](https://help.globee.com/)
  * GloBee merchant support documentation

**Ecwid Support**

* [Homepage](https://www.ecwid.com/)
* [Documentation](https://help.ecwid.com/)
* [Support](https://help.ecwid.com/customer/portal/emails/new)

## Version History

- Bitpay plugin version 1.0
- Tested against Ecwid version 13.0.1629
- Added new HTTP header for version tracking
