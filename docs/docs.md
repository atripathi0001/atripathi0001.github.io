This is the guide to install Ruby
https://jekyllrb.com/docs/installation/

### I assume you have already downloaded and installed Ruby. Here’s what you need to do next:

- Run <code>gem install jekyll bundler</code>.
- Copy the repo in your desired folder.
- Enter into the folder by executing <code>cd name-of-the-folder</code>.
- Run <code>bundle install</code>.
- If you want to access and customize the project, use <code>bundle exec jekyll serve</code>. This way it will be accessible on <code>http://localhost:4000</code>.

For more info, https://jekyllrb.com/docs/

### Now the project would be running locally

One thing to remember - true is on, false is off.

#### Adding new Post

Add YYYY-MM-DD-blog-post-name.md to _posts/.
Add front matter to the top of your new blog post file.

```
---
layout: post
title: Awesome Title
date: YYYY-MM-DD HH:SS
category: blog
tag:
- tag 1
- tag 2
image: /assets/images/markdown.jpg #path for the image
headerImage: false #to disable or enable the header image
star: false #if true will give a blue color gradient on the title on blog listing page
author: authorname  #author name written same in _config.yml Eg.abhishektripathi
description: Write blog-post description here, if you left this empty the blog-post description will be the first 25 words of the blog-post body.
---
```

Your blog post content goes there. You need to write the in markdown format. You can include text, images, video and all here.
For more info, https://jekyllrb.com/docs/posts/#creating-post-files

#### Adding new Project

Add YYYY-MM-DD-project-name.md to _posts/.
Add front matter to the top of your new project file.

```
---
layout: post
title: Awesome Title
date: YYYY-MM-DD HH:SS
category: blog
tag: tag 1
projects: true (This will tell that the current blog post is project.)
hidden: false (It will not be count this post in blog pagination)
image: /assets/images/markdown.jpg (path for the header image)
headerImage: false (to disable or enable the header image)
star: false (if true will give a blue color gradient on the title on blog listing page )
author: authorname (author name written same in _config.yml Eg.abhishektripathi)
description: Write blog-post description here, if you left this empty the blog-post description will be the first 25 words of the blog-post body.
externalLink: false
---
```
The new project will be added to the project list page of your project.
Check more project templates from here.

### Google Analytics
To integrate Google Analytics, open _includes/analytics-google.html, and add your Google Analytics code.

