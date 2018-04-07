# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) WordPress  3.7-4.4 - Authenticated Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.6
  - [x] GIF Walkthrough: <img src="https://raw.githubusercontent.com/cheezm91/CodePathWeek7/master/1XSS.gif" width="800">
  - [x] Steps to recreate: 
    - Log in as admin
    - Create new post
    - Post link and add alert script. Ex: http://www.example.com/wp-admin/customize.php?theme=<svg onload=alert('HACKED')>
    - Publish and view page
  - [x] Affected source code: 
    - [Link 1](https://github.com/WordPress/WordPress/commit/7ab65139c6838910426567849c7abed723932b87)
2. (Required) WordPress <= 4.2 - Unauthenticated Stored Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [x] GIF Walkthrough: <img src="https://raw.githubusercontent.com/cheezm91/CodePathWeek7/master/2XSS.gif" width="800">
  - [x] Steps to recreate: 
    - Comment on post with:
     <a title='x onmouseover=alert(1) style=position:absolute;left:0;top:0;width:5000px;height:5000px  AAAAAAAAAAAA...[64 kb]..AAA'></a>
    - Text must be over 64 kb
    - Wait for admin to approve of comment
1. (Required) WordPress  3.7-4.4 - Authenticated Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.6
  - [x] GIF Walkthrough: <img src="https://raw.githubusercontent.com/cheezm91/CodePathWeek7/master/1XSS.gif" width="800">
  - [x] Steps to recreate: 
    - Log in as admin
    - Create new post
    - Post link and add alert script. Ex: http://www.example.com/wp-admin/customize.php?theme=<svg onload=alert('HACKED')>
    - Publish and view page
  - [x] Affected source code: 
    - [Link 1](https://github.com/WordPress/WordPress/commit/7ab65139c6838910426567849c7abed723932b87)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

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
