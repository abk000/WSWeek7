# Project 7 - WordPress Pentesting

Time spent: **3** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Authenticated Cross Site Scripting 
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [X] GIF Walkthrough:
    <img src="https://i.imgur.com/XshEAAh.gif">
  - [X] Steps to recreate: 
    - As an admin, create new post. 
    - Embed JavaScript into an HTML link tag. 
    - When published, the user will receive a pop-up when hovering over the link. 
  - [] Affected source code:
2. (Required) Cross Site Scripting Through Comments
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough:
    <img src="https://i.imgur.com/wXFKzrb.gif">
  - [X] Steps to recreate:
    - Logged in as an administrator, go to a post. 
    - Comment a script tag with Javascript alert function. 
    - Pop-up will appear upon each load. 
  - [] Affected source code:
3. (Required) Using login error messages to obtain valid usernames
  - [X] Summary: 
    - Vulnerability types: User enumeration
    - Tested in version: 4.2
    - Fixed in version: 4.2.9
  - [X] GIF Walkthrough:
     <img src="https://i.imgur.com/fpCqpdv.gif">
  - [X] Steps to recreate:
     - Try to login as admin with an incorrect password; error message tells you the password doesn't mach the user, revealing that's a valid username. 
     - Try to login with another username; if the user does not exist, you receive an 'invalid username' error. 
  - [X] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/blob/4.2-branch/wp-login.php)
4. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
5. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

## Notes

## License

    Copyright [2018] [Arslan Saeed]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
