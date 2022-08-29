title: History
slug: history
date: 2022-08-26 12:02:45 UTC+12:00
tags: 
category: 
link: 
description: 
type: text
hidetitle: true
<!---
Draft completed: 2022-08-28 Ian Stewart

TODO: More Historical info???

TODO> When moved to WLUG repo
Future: Change https://github.com/irsbugs/wlug.github.io/tree/src
to https://github.com/WLUG/wlug.github.io/tree/src

and change: https://github.com/irsbugs/wlug.github.io
to: https://github.com/WLUG/wlug.github.io

and change: https://irsbugs.github.io
to: ttps://wlug.github.io

Add the yaml script to updates the website automatically, etc.
workflow *yaml* code in the src branch file .github/workflows

on: [push]

jobs:
  nikola_build:
    runs-on: ubuntu-latest
    name: 'Deploy Nikola to GitHub Pages'
    steps:
    - name: Check out
      uses: actions/checkout@v2
    - name: Build and Deploy Nikola
      uses: getnikola/nikola-action@v3
      with:
        dry_run: false

-->

# History and General Information

## Wiki

In 2002 WLUG became an incorporated society and at the same time a [Wiki](https://en.wikipedia.org/wiki/Wiki) was set up to aid Linux and Open Source enthusiasts. At the time Daniel Lawson was the president of WLUG. Daniel continues to keep the *WLUG wiki* running on his servers.

Feel free to take a walk back in time and browse the [WLUG wiki](http://wiki.wlug.org.nz/)


## Creation of this WLUG Website

This website has been created using the Python based [Nikola](https://getnikola.com/) *Static Site Generator*. This is open source software and you may view the github repository for the [source code](https://github.com/getnikola/nikola).

The source files used for *Nikola* to build this website reside at the WLUG repository wlug.github.io [src branch](https://github.com/irsbugs/wlug.github.io/tree/src), while the website html files reside in the [main branch](https://github.com/irsbugs/wlug.github.io)

Those with access to the WLUG repository wlug.github.io may have a local [git](https://en.wikipedia.org/wiki/Git) folder that holds a copy of the source and main website files. These files may then be edited to enhance the website and using the *nokola gihub_deploy* bash command the files on github are updated. 

GitHub also provide web-hosting service and this WLUG website is accessed via [https://wlug.github.io](https://irsbugs.github.io).

Using a [CNAME record](https://en.wikipedia.org/wiki/CNAME_record) the DNS is able to map **wlug.org.nz** to **wlug.github.io**. Users connecting to **https://wlug.org.nz** will be unaware that they are connected to a github hosted website.

Another feature of GitHub is that using a browser a change may be made to the website source code. For example a change of phone number. Upon committing the change, GitHub will run the Nikola updating process. After a few minutes the web-site will be updated. This is done by the workflow [yaml code](https://getnikola.com/blog/automating-nikola-rebuilds-with-github-actions.html) in the src branch file .github/workflows/main.yml.
 
            







