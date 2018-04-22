# Project 7 - WordPress Pentesting

Time spent: **7** hours spent in total

> Objective: "Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress
are injected into otherwise benign and trusted web sites XSS attacks occur when an attacker uses a web application
to send malicious code, generally in the form of a browser side script, to a different end user."

## Pentesting Report

1. XSS
  - [X] Summary:Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected into
  otherwise benign and trusted web sites. This was a 'mouseover' XSS used to inject code into this user post.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.11
  - [X] GIF Walkthrough: 
       ![](https://github.com/neltoms/cybersecurity/blob/master/Week_7/GIF/XSS.gif)
  - [X] Steps to recreate: See Walkthrough
  - [X] Affected source code: ```view-source:http://wpdistillery.vm/sample-page/)```
 
1. User List Table Enumeration
  - Summary: User enumeration vulnerability exploit using wpscan enumeration flag to identify usernames
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version: 4.3.1
  - [X] GIF Walkthrough: 
      ![](https://github.com/neltoms/cybersecurity/blob/master/Week_7/GIF/username_enum.gif)
  - [X] Steps to recreate: See Walkthrough
  - [X] Affected source code:```view-source:http://wpdistillery.vm/sample-page/)```
  
1. Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
  - [X] Summary: Used XSS embedded in YouTube video URL within a user's post
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [X] GIF Walkthrough: 
    ![](https://github.com/neltoms/cybersecurity/blob/master/Week_7/GIF/embedded_post.gif)
  - [X] Steps to recreate: See Walkthrough
  - [X] Affected source code:```view-source:http://wpdistillery.vm/sample-page/)```

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes
There were challenges setting up the vulnerability testing software.

## License

    Copyright 2018 Nel Toms

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
