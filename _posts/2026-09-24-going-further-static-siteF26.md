---
title: "Going Further with Your Static Site F26"
last_modified_at: 2026-09-24T12:00:00-05:00
tags:
  - Github pages
  - Markdown
  - Interactive Map
  - R
  - F26
---

## Going Further with Your Static Site F26

This post explains some more things we can do with our site. 

## So far

So far we know how to 

- fork a repo containing a template
- create a page
- edit the navigation.yml file and the config.yml file to organize our site
  
## New topics 

- creating a post and tagging the post
- inserting an interactive map using an iframe
- inserting an image in a page or post
- (setting the landing page beyond the default)
- (creating a table of contents for a page)

## Creating a post

The only parts which are complex here are (1) making sure you have the right `yml` header and (2) naming the file correctly. 

Let's look at the name of this very post and its yml header. 

```
---
title: "Going Further with Your Static Site F26"
last_modified_at: 2026-09-24T12:00:00-05:00
tags:
  - static sites
  - Markdown
  - Interactive Map
  - R
  - F26
---
```
It contains a title, modified date, and tags. Minimal mistakes allows us to use both tags and categories. Think of categories as the main chapters or folders that broadly organize your site into a few big topics, while tags are the specific index terms or keywords that describe the exact details inside a post.

I find that both too much for our purposes in one semester. I would suggest that you create a post now, reuse this header and add some tags. The tags index is created automatically when you commit changes and rebuild your site. 

Tagging is an art and you may revise them over time. In general it makes finding content by its topic easier. 

You will do assignments as posts. _So go ahead and create four posts for the assignments._ 

## Inserting an interactive map using an iframe

In Assignment 1, we use a notebook that creates a "standalone" map in html. We need to host that map on Github and then call it up using an iframe. 

1. Go to your assets folder and add a subfolder called `maps`. You can do that in VSCode. 
2. Take the `html` you create at the end of the notebook and export it from posit.cloud. Export is found under the settings icon.
3. Drag and drop that `html` file into the maps subfolder you created in assets. Commit these changes.

Make sure that you can see the map, formatted like this https://djwrisley.github.io/DHS/assets/maps/LB_featuremap-2.html

4. Now we create an iframe.

{% raw %}
```
<div style="width:100%; height:70vh;">
  <iframe
    src="{{ '/assets/maps/nameofyourmap.html' | relative_url }}"
    style="width:100%; height:100%; border:0;"
    loading="lazy">
  </iframe>
</div>
```
{% endraw %}

The `div` is a container for the map with some parameters specifying how much space is alloted to the map in the theme. 100% means the full allocation of the containing element of the theme. 

<div style="width:100%; height:70vh;">
  <iframe
    src="{{ '/assets/maps/LB_featuremap-2.html' | relative_url }}"
    style="width:100%; height:100%; border:0;"
    loading="lazy">
  </iframe>
</div>

## Inserting an image in your post. 

It is easy to put screenshots or other images you have that you want into your posts or pages.

Create an images folder in assets and then place any image you want to use in it.

Within the markdown, use this syntax: 

```
<img src="/assets/images/imagename.png|jpg" style="zoom:50%;" />
```


Good luck with your customization!


