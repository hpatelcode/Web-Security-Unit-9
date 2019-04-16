# Project 8 - Pentesting Live Targets

Time spent: **5** hours spent in total

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

Vulnerability #1: SQL Injection: Inserting an SQL Query to make the website wait a certain seconds before returning.
![blue1](https://user-images.githubusercontent.com/25422131/56177369-62f98e80-5fcc-11e9-878f-b451b80eac8e.gif)


Vulnerability #2: Session Hijacking/Fixation: The session ID is found from the chrome developer tools console. You can gain access to the said session by providing the corresponding ID.
![blue2](https://user-images.githubusercontent.com/25422131/56177469-bf5cae00-5fcc-11e9-82ad-c7e4aa0437f6.gif)


## Green

Vulnerability #1: User Enumeration: Invalid usernames + password combinations error message is displayed in regular text meanwhile correct username + incorrect password combinations error messages are displayed bold.
![green1](https://user-images.githubusercontent.com/25422131/56177573-1e222780-5fcd-11e9-882d-6390c34383d3.gif)

Vulnerability #2: Cross-Site Scripting (XSS): The feedback text box allows scripts to be inputted by users. 
![green2](https://user-images.githubusercontent.com/25422131/56177669-722d0c00-5fcd-11e9-8d37-207bbc6db896.gif)


## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR): Changing the value of the "id=" (ex. 11,12,13) at the end of the URL gives access to people that were not shown in the list before. 
![red1](https://user-images.githubusercontent.com/25422131/56177764-c89a4a80-5fcd-11e9-82e0-7ca903aa63e6.gif)

Vulnerability #2: Cross-Site Request Forgery (CSRF): Editing the CSRF token for the form should not finalize the request. However, changing the CSRF token for a form on the Red challenge allows the request to be submitted. 
![red2](https://user-images.githubusercontent.com/25422131/56177889-40687500-5fce-11e9-89c9-eb930f5cad24.gif)

## Notes

Describe any challenges encountered while doing the work
