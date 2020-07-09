## Laravel

Sales of Point Framework Laravel with Infyom Laravel Generator (custom login)
Minimal PHP 7.1 > requirement PHP 7.2.32

How to use:
- Download repository and extracted or clone the repository
	```sh
	$ git clone https://github.com/fredriclesomar/EPoS.git
	```
- Running composer
	```sh
	$ cd EPoS
	$ composer install
	```
- Setting .env dan key application
	```sh
	$ nano .env
	$ php artisan key:generate
	```
- Edit database name, database username dan database password

	> DB_DATABASE=your_db.

 	> DB_USERNAME=your_mysql_username.
 	
	> DB_PASSWORD=your_mysql_password.

- Migrate table
	```sh
	$ php artisan migrate
	```

- Open browser di 127.0.0.1:8000
- Register new account
- Login

Note.Security Issue:
Remediation

Upgrade symfony/http-foundation to version 4.2.12 or later.
=====================================
"require": {
  "symfony/http-foundation": "4.2.12"
}
=====================================


#CVE-2019-10913
critical severity
Vulnerable versions: >= 4.0.0, < 4.1.12
Patched version: 4.1.12

In Symfony before 2.7.51, 2.8.x before 2.8.50, 3.x before 3.4.26, 4.x before 4.1.12, and 4.2.x before 4.2.7, HTTP Methods provided as verbs or using the override header may be treated as trusted input, but they are not validated, possibly causing SQL injection or XSS. This is related to symfony/http-foundation.


#CVE-2019-18888
moderate severity
Vulnerable versions: >= 4.0.0, < 4.2.12
Patched version: 4.2.12

An issue was discovered in Symfony 2.8.0 through 2.8.50, 3.4.0 through 3.4.34, 4.2.0 through 4.2.11, and 4.3.0 through 4.3.7. If an application passes unvalidated user input as the file for which MIME type validation should occur, then arbitrary arguments are passed to the underlying file command. This is related to symfony/http-foundation (and symfony/mime in 4.3.x).
