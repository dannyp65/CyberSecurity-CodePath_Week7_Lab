# Project 7 - WordPress Pentesting

Time spent: 2 hours spent in total

> Objective: Find, analyze, recreate, and document three affecting an old version of WordPress

## Pentesting Report

1. Unauthenticated Stored Cross-Site Scripting
  - [ ] Summary: 
        This vulnerability can be use by unauthenticate user through comment section of WordPress, the attacker inject Javascript code in the comment, the code will be trigger when the comment is viewed by Admin. 
        
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: 
  
    - [Link 1](http://klikki.fi/adv/wordpress2.html)
1. Authenticated Stored Cross-Site Scripting 
  - [ ] Summary: The vulnerability allows a user with posting previlage to comprimise the website. The attacker can insert a  HTML containing Javascript into a post.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: 

    - [Link 2](https://klikki.fi/adv/wordpress3.html)
1. (Required) Large File Upload Error XSS
  - [ ] Summary: The attacker can inject a maliciuos script into the filname, WordPress didn't senitize the filename string, so when the victim upload the file the malicous script will be trigger.
    - Vulnerability types: XSS
    - Tested in version:4.2
    - Fixed in version: 4.2.15
  - [ ] GIF Walkthrough: 

    - [Link 3](https://hackerone.com/reports/203515)


## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

The Lab is fun. It took time to crecreate the attacks. 

## License

    Copyright [yyyy] [Nhan PHam]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
