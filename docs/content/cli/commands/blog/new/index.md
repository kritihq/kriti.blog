---
title: New Blog
author: Vinay Gaykar
publishDate: 26-09-2024
draft: false
---

__Usage:__ `kriti new blog`

---

These command will create new blog within your portfolio.

While creating new blog two inputs are expected from the user:

1. __title__: The blog title, which must be unqiue across all blogs hosted on this platform
2. __source__: Location of folder which contains the markdown files, this folder follows a [required structure]({{< ref "/content/structure" >}} "Content Structure")

Following is a step by step guide to using `new` command to register a blog.
Verify _Kriti_ is already installed on your machine, if not follow the [Quick start guide]({{< ref "/quick-start" >}}) till the installation section.

> TIP: Append `--help` to any command to get available help without executing the command itself
> Example: `kriti --help` will return help for the complete application and `kriti new blog --help` will provide help only for `new` command


## Guide to `new blog`

Run following command `kriti new blog` to get started.

### Blog title
A prompt will apear to enter blog's title. Title is a unique identifier across all the blogs hosted on this platform. It will also dictate the URL generated for the blog.
So if title provided is _example_ then generated URL will be `https://example.kriti.blog` and no other blog can use the _example_ as title until this blog is deleted.

### Locating the blog contents

Next prompt will be to confirm if sample content should be generated.

#### Generating sample content

This is an optional step and must be used if there is no content ready for the blog. 
Kriti will create a sample blog content which shows off different possible scenarios and few tricks. A mini documentation of sorts.

Select "Yes" or press "y" key to proceed or "n" key to cancel this step.
Now select the folder where this content should be placed. Use up/down arrow keys to iterate through available folders, right arrow key to open a folder, left arrow key to exit and enter key to select current folder to be used where the sample content will be placed.

This sample content is full fledged and user can directly proceed with publishing if needed.

#### Selecting already available content

If content is already available to publish then there is no need to generate sample content.
A folder picker will show up to select the folder which has the blog content. Use up/down arrow keys to iterate through available folders, right arrow key to open a folder, left arrow key to exit and enter key to select current folder.

> Remember to select the parent folder of _content_ folder not the _content_ folder itself.

### Done!

Blog is registered! its URL will be displayed on screen.

Next steps would be to either of:

1. [Publish the blog]({{< ref "/cli/commands/blog/publish" >}})
2. [List all blogs]({{< ref "/cli/commands/blog/list" >}})
3. [Delete the blog]({{< ref "/cli/commands/blog/delete" >}})

