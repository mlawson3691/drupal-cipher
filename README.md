# Shift Cipher

#### A Drupal 7 app with a custom module, December 2nd, 2016

#### By Mark Lawson

## Description

This application is an exercise in Drupal 7 creating a custom module. The application serves as a shift cipher, where users enter a shift value, shift direction, and text to encrypt. After validating the user's input, the text is encrypted and returned on a new page.

## Specifications

* The application will replace a letter based on the shift parameters
  * Example Input: 'a', 1, 'right'
  * Example Output: 'b'

* The application will replace a string based on the shift paramaters
  * Example Input: 'dog', 1, 'left'
  * Example Output: 'cnf'

* The application will account for the start and end of the alphabet
  * Example Input: 'z', 1, 'right' AND 'a', 1, 'left'
  * Example Output: 'a' AND 'z'

* The application will maintain punctuation and spacing from the origin string
  * Example Input: 'hi there!', 1, 'left'
  * Example Output: 'gh sgdqd!'

* The application will return a string in all lowercase characters
  * Example Input: 'Dog', 1, 'left'
  * Example Output: 'cnf'

* The application will prevent invalid input in all fields of the form
  * Example Input: 'Dog', -5, 'up'
  * Example Output: false

## Setup/Installation Instructions

* Clone the repository
* Start a server using MAMP (on Mac)
* Open the MAMP Preferences:
  * Set the document root to the project's root directory
  * Set the Apache Port to 8888 and the MySQL Port to 8889
* Set up the database:
  * In the browser, navigate to phpMyAdmin (localhost:8888/phpMyAdmin)
  * Select the "Import" tab along the top
  * Choose the .sql.zip file from the project located in sites/db-backup
  * Make sure character set is "utf-8"
  * Click "Go"
  * Select the "Privileges" tab along the top
  * Click "Add User" and enter the following credentials:
    * Username: cipher
    * Host: Local
    * Password: cipher
  * Click "go"
* Navigate your browser to localhost:8888
* NOTE: Before committing again, be sure to export database and replace copy in sites/db-backup

## Known Bugs

There are no known bugs at this time.

## Support and Contact Details

Please report any bugs or issues to mlawson3691@gmail.com.

## Languages/Technologies Used

* Drupal 7.52
* MAMP
* MySQL

### License

*This application is licensed under the MIT license.*

Copyright (c) 2016 Mark Lawson
