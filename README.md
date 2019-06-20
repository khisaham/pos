[ ![Download](https://github.com/khisaham/pos/archive/master.zip) ](https://github.com/khisaham/pos/archive/master.zip)
[![Build Status](https://github.com/khisaham/pos/archive/master.zip)](https://github.com/khisaham/pos/archive/master.zip)
[![Join the chat at https://gitter.im/pos](https://github.com/khisaham/pos/archive/master.zip)
[![devDependency Status](https://github.com/khisaham/pos/archive/master.zip)
[![GitHub version](https://github.com/khisaham/pos/archive/master.zip)
[![Translation status](https://github.com/khisaham/pos/archive/master.zip)](https://github.com/khisaham/pos/archive/master.zip)


Introduction
------------

Point of Sale is a web based point of sale system.
The main features are:
* Stock management (Items and Kits)
* VAT, customer and multi tiers taxation
* Sale register with transactions logging
* Quotation and invoicing
* Expenses logging
* Receipt and invoice printing and/or emailing
* Barcode generation and printing
* Suppliers and Customers database
* Multiuser with permission control
* Reporting on sales, orders, expenses, inventory status
* Receivings
* Giftcard
* Rewards
* Restaurant tables
* Messaging (SMS)
* Multilanguage
* Selectable Boostrap (Bootswatch) based UI theme
* Mailchimp integration
* reCAPTCHA to protect login page from brute force attacks
* GDPR ready

The software is written in PHP language, it uses MySQL (or MariaDB) as data storage back-end and has a simple but intuitive user interface.

The latest 3.x version is a complete overhaul of the original software.
It is now based on Bootstrap 3 using Bootswatch themes, and still uses CodeIgniter 3 as framework.
It also has improved functionality and security.

Deployed to a Cloud it's a SaaS (Software as a Service) solution.

Installation
------------

Please **refrain from creating issues** about installation issues **before reading the FAQ and going through existing github issues**. We have a build pipeline that checks the sanity of our latest repository commit and in case the application itself is broken then our build will be as well.

This application **can be setup in many different ways** and we only **support the ones described in the INSTALL file linked below**.

Read the [INSTALL.md](https://github.com/khisaham/pos/blob/master/INSTALL.md) in our repository.


License
-------

Open Source Point of Sale is licensed under MIT terms with an important addition:

_The footer signature "You are using Open Source Point Of Sale" with version, 
hash and link to the original distribution of the code MUST BE RETAINED, 
MUST BE VISIBLE IN EVERY PAGE and CANNOT BE MODIFIED._

Also worth noting:

_The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software._

For more details please read the file [LICENSE](https://github.com/khisaham/pos/blob/master/LICENSE).

It's important to understand that althought you are free to use the software the copyright stays and the license agreement applies in all cases.
Therefore any actions like:

- Removing LICENSE and any license files is prohibited
- Authoring the footer notice replacing it with your own or even worse claiming the copyright is absolutely prohibited
- Claiming full ownership of the code is prohibited

In short you are free to use the software but you cannot claim any property on it.

Any person or company found breaching the license agreement will have a bunch of monkeys at the door ready to destroy their servers.



Reporting Bugs
--------------

If you are taking a release candidate code please make sure you always run the latest database upgrade script and you took the latest code from master.
Please DO NOT post issues if you have not done those step.

Bug reports must follow this schema:

1. pos **version string with git commit hash** (see ospos footer)
2. POS name and version running your Web Server (e.g. CentOS 6.9, Ubuntu 16.4, Windows 10)
3. Web Server name and version (e.g. Apache 2.2, Apache 2.4, Nginx 1.12, Nginx 1.13)
4. Database name and version (e.g. MySQL 5.5, MySQL 5.6, MySQL 5.7, MariaDB 10.0, MariaDB 10.1, MariaDB 10.2)
5. PHP version (e.g. 5.6, 7.0, 7.1, 7.2)
6. Language selected in OSPOS (e.g. English, Spanish)
7. Any configuration of OSPOS that you changed
8. Exact steps to reproduce the issue (test case)
9. Optionally some screenshots to illustrate each step

If above information is not provided in full, your issue will be tagged as pending.
If missing information is not provided within a week we will close your issue.


FAQ
---

* If you are seeing the message **system folder missing**, then you have cloned the source using git and you need to run a build *first*. Check [INSTALL.md](https://github.com/khisaham/pos/blob/master/INSTALL.md) for instructions.

* If at login time you read "The installation is not correct, check your php.ini file.", please check the error_log in public folder to understand what's wrong and make sure you read the [INSTALL.md](https://github.com/khisaham/pos/blob/master/INSTALL.md).


* Apache server configurations are SysAdmin issues and not strictly related to POS. Please make sure you first can show a "hello world" html page before pointing to OSPOS public directory. Make sure .htaccess is correctly configured.

* If the avatar pictures are not shown in Items or at Item save time you get an error, please make sure your public and subdirs are assigned to the correct owner and the access permission is set to 755.

* If you install ospos in docker behind a proxy that performs ssloffloading, you can enable the url generated to be https instead of http, by activating the environment variable FORCE_HTTPS = 1.


Credits
-------
|JetBrains|Travis CI|
|:-:|:-:|
|![IntelliJ IDEA](https://raw.githubusercontent.com/wiki/j-easy/easy-batch/images/logo/intellijidea-logo.png)|[Travis CI](https://travis-ci.com/images/logos/TravisCI-Full-Color.png)|
|Many thanks to [JetBrains](https://www.jetbrains.com/) for providing a free license of [IntelliJ IDEA](https://www.jetbrains.com/idea/) to kindly support the development of POS|Many thanks to [Travis CI](https://travis-ci.org) for providing a free continuous integration service for open source projects.|
