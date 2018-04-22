# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: **_SQLI_**

**Description**: The Blue site, unlike the others, allowed me to determine if an SQL injection is possible by returning the message **_Database query failed_**. With enough time and the proper syntax/injection, this site can be breached.

**GIF Walkthrough**:
![](https://github.com/neltoms/cybersecurity/blob/master/Week_8/GIF/SQLI.gif)

Vulnerability #2: __________________


## Green

Vulnerability #1: **_Username Enumeration_**

**Description**: When the username of someone in the database is entered, the '**Log in was unsuccessful**' is displayed in bold type but displayed in plain type when not in the database. The other two sites were consistently bold regardless of whether the user was in the system or not.

**GIF Walkthrough**:
![](https://github.com/neltoms/cybersecurity/blob/master/Week_8/GIF/username_enum.gif)

Vulnerability #2: **_XSS_**

**Description**: The Green site allowed me to insert a working link into the _Feedback_ form which executes upon the admin opening the form. The other two site converted the script into harmless text which did not execute upon accessing.

**GIF Walkthrough**:
![](https://github.com/neltoms/cybersecurity/blob/master/Week_8/GIF/XSS.gif)


## Red

Vulnerability #1: **_IDOR_**

**Description**: The URL is vulnerable in all 3 sites by allowing a user to manipulate the **_id_** to shuffle through salespeople in the organization, but it is especially vulnerable with the red site, which allows you to access inactive users, thus harvesting potentially damning information.

**GIF Walthrough**:
![](https://github.com/neltoms/cybersecurity/blob/master/Week_8/GIF/IDOR.gif)

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work

