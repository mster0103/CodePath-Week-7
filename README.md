# Project 7 - WordPress Pentesting

Time spent: 3 hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) XSS
  - [ ] Summary: Was able to successfully make an XSS alert through making a post
    - Vulnerability types: XSS
    - Tested in version: 4.1.4
    - Fixed in version: 
  - [ ] GIF Walkthrough: <img src='https://github.com/mster0103/CodePath-Week-7/blob/master/PostXSS.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

  - [ ] Steps to recreate: Create a new post and type <script> alert("XSS Vulnerability"); </script> and the alert will display when viewing the post 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
1. (Required) XSS 
  - [ ] Summary: Was able to successfully make an XSS alert through making a comment
    - Vulnerability types: XSS
    - Tested in version: 4.1.4
    - Fixed in version: 
  - [ ] GIF Walkthrough: <img src='https://github.com/mster0103/CodePath-Week-7/blob/master/CommentXSS.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [ ] Steps to recreate: Create a new comment and type <script> alert("XSS Vulnerability"); </script> and the alert will diplay when posting the comment
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
1. (Required) XSS
  - [ ] Summary: Was able to make a post with a possibly malicious XSS through mouse over
    - Vulnerability types: XSS
    - Tested in version: 4.1.4
    - Fixed in version: 
  - [ ] GIF Walkthrough: <img src='https://github.com/mster0103/CodePath-Week-7/blob/master/postclickXSS.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [ ] Steps to recreate: Create a new post and type <b onmouseover=alert('exploitmeplease')>click me!</b>
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Installing wordpress distillery came with come complications

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
