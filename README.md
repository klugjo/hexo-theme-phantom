# Phantom Blog Hexo

![](http://www.codeblocq.com/img/hexo-theme-thumbnail/Phantom.png)

Hexo implementation of the free [HTML5Up Phantom Template](http://html5up.net/phantom)

Phantom is a photography/design portfolio oriented, responsive theme. [Demo here](http://www.codeblocq.com/assets/projects/hexo-theme-phantom/).

## Features Overview

- Disqus and Facebook comments
- Google Analytics
- Cover image for posts and pages
- Tags Support
- Responsive Images
- Image Gallery
- Social Accounts configuration
- Pagination

## Not Supported

- Post Categories will not be displayed
- Posts and Pages Dates will not be displayed

## External libraries used

- [FeatherLight.js](http://noelboss.github.io/featherlight/) (Gallery)
- [jQuery](https://jquery.com/)
- [Skel](https://github.com/n33/skel)

## Installation

### SCSS support

Phantom uses SCSS as a css preprocessor. SCSS is not supported by default in hexo, the `hexo-renderer-scss` is required.

Install it by using:

```
$ npm install --save hexo-renderer-scss
```
### Install the theme

Install the theme by using:

```
$ git clone https://github.com/klugjo/hexo-theme-phantom themes/phantom
```

Then update your blog's main `_config.yml` to set the theme to `phantom`:

i.e:

```
# Extensions
## Plugins: http://hexo.io/plugins/
## Themes: http://hexo.io/themes/
theme: phantom
```

## Theme Configuration

The theme's global configuration is done in `/themes/hexo-theme-phantom/_config.yml`.

### Menu

The menu is configured in the theme's `_config.yml`.

```
# Header
menu:
  Home: /
  Archives: /archives
  About: /about.html
```

The object key is the label and the value is the path.

### Blog's Logo Image Source

The blog's logo (next to blog title) is configured in the theme's `_config.yml`.

```
# Logo Image Source
logo_src: /images/logo.svg
```

### Blog's Main Subtitle

The blog's main subtitle (text just below the logo) is configured in the theme's `_config.yml`.

```
# Theme Main Subtitle
subtitle_main: This is Phantom, a free, fully responsive site<br />template designed by <a href="http://html5up.net">HTML5 UP</a>.
```

### Blog's Second Subtitle

The blog's second subtitle (smaller text below the logo) is configured in the theme's `_config.yml`.

```
# Theme Secondary subtitle
susbtitle_secondary: Etiam quis viverra lorem, in semper lorem. Sed nisl arcu euismod sit amet nisi euismod.
```

### Footer About Section Text

The About section's text in the footer is configured in the theme's `_config.yml`.

```
# Footer About Section
about_footer: This theme was initially developed by HTML5 Templates and adapted for Hexo by Jonathan Klughertz.
```

### Default post title

The default post title (used when no title is specified) is configured in the theme's `_config.yml`.

```
# Default post title
default_post_title: Untitled
```

### Default index page cover image

You can specify a default thumbnail for posts on the index page (Home page). This image will be used if you forget to specify an image in the post's front matter.

```
# Default post cover index page
default_cover_index: "http://placehold.it/450x450"
```

### Default post page cover image

You can specify a default thumbnail for posts/pages on the post/page page (Detail Page). This image will be used if you forget to specify an image in the post's front matter. If you don't specify a default and you don't specify an image in your post, no image will be displayed

```
# Default post cover index page
default_cover_detail: "http://placehold.it/1300x500"
```

### Show Dates

By default, Phantom does not show dates for posts and pages. You can set this config to true if you need to.

```
# Show Dates for posts and pages
show_dates:
```

### Comments

The comments provider is specified in the theme's `_config.yml`. If you specify both a `disqus_shortname` and a `facebook.appid` there will be 2 sets of comment per post. So choose one.

```
# Comments. Choose one by filling up the information
comments:
  # Disqus comments
  disqus_shortname: klugjotest
  # Facebook comments
  facebook:
    appid: 123456789012345
    comment_count: 5
    comment_colorscheme: light
```

### Google Analytics

The Google Analytics Tracking ID is configured in the theme's `_config.yml`.

```
# Google Analytics Tracking ID
google_analytics:
```

### Social Account

Setup the links to your social pages in the theme's `_config.yml`. Links are in the footer.

```
# Social Accounts
twitter_url: 
facebook_url: https://www.facebook.com/
instagram_url: 
dribble_url: https://dribbble.com/pixelhint
github_url: 
googleplus_url: https://plus.google.com/+Pixelhint/posts
behance_url: https://www.behance.net/
fivehundredpx_url: 
email_url: 
rss_url: 
```

## Post Custom Configuration

For each post, you can specify additional information in the [front matter](https://hexo.io/docs/front-matter.html)

### Post's Subtitle

Use `subtitle` to specify the text that will be displayed below the title on the Home Page.

```
subtitle: Lorem Ipsum
```

### Post's Index Thumbnail

Use `cover_index` to specify an image that will be used for that post on the Home page (also knows as index)

Example:

```
cover_index: /assets/work1.jpg
```

### Post's Detail Thumbnail

Use `cover_detail` to specify an image that will be used for that post on the Detail page for that post.

```
cover_detail: /assets/hero_image.jpg
```

## Creator

This theme was created by [HTML5 Up](http://html5up.net/phantom/) and adapted for Hexo by [Jonathan Klughertz](http://www.codeblocq.com/).

## Bugs

If you have a question, feature request or a bug you need me to fix, please [click here](https://github.com/klugjo/hexo-theme-phantom/issues/new) to file an issue.