---
title: Quick Start
description: A short document to quikly publish your first blog
summary: quickly, please!
draft: false
---

This page will help you get started with Kriti from setting up and login/signup to publishing your blog.

## Installing CLI

Basically Kriti converts the markdown (.md) files into site pages (.html). To achieve this you'll need to install the application locally.

Use below commands based on your OS, they will take care of downloading and installing necessary software.

### Mac OS or Linux

Open _Terminal_ app and run following command

```console
curl -sSfL https://kriti.blog/downloads/kriti-cli/latest | bash
```

### Windows

Open _Powershell_ (recommended) or _Command Prompt_ and run following command

```console
powershell -Command "& {Invoke-WebRequest -UseBasicParsing -MaximumRedirection 5 'https://kriti.blog/downloads/kriti-cli/latest?os=windows' | Invoke-Expression}"
```


Close the terminal window and reopen it again to perform verification.
Verify installation by running  `kriti version`  which should print something like _vx.y.z_. Anything else means installation failed.


## Registration and Login

Run `kriti login` to login to your account. This will open new web page for authentication, new account will be created if you are a new user


## Publishing blogs

Now that all the setup is completed we can get started with publishing a blog.

We know nobody likes to remember commands so we made them as easy as typing a sentence (until UI is ready, stay tuned)

### Blog content

Download sample blog folder from [here](https://github.com/vinaygaykar/sample-blog.kriti.blog/archive/refs/heads/main.zip). This zip showcases ideal blog structure.

Basic idea is:

- All blogs go under _content_ folder
- Every blog has its own folder under _content_

### Creating new blog

- Run `kriti new blog`
- Enter blog title. Title must be unique and will be used to generate the URL for this blog. Only alphabets are allowed (no numbers, symbols and spaces)
- Select _yes_ if you want to generate a sample blog
- Choose where the blog content is located on your machine
- Done

Thats it! blog will be hosted at `https://{blog title}.kriti.blog`


## Done! Up next?

Try adding new blog by updating the _content_ folder.

__TIP!__ Add `draft: true` to any blog's frontmatter to make it disappear from your site but not deleted from the machine.

