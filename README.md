Will's Food Blog
========

Forked from Mediator

Features
-------
* Fully Responsive layout
* Use header images in articles, if you want to (add tag "image" and url to the image in the front matter section of a post)
* Minimal design
* Featured article support
* FontAwesome implemented for easy use of icons fonts
* Free & Open Source Font usage

I Added

* Jekyll compose for command line composing
* Jekyll Sitemap for potential SEO improvements

TODO

* Topic/Tag/Category pages
* OpenGraph?
* Embeds?
* Analytics
* Search Console
* AMP?

Getting Started
---
- Clone this repository
- Install the requried gems: `bundle install`
- Run the jekyll server: `bundle exec jekyll serve --drafts`

You should have a server up and running locally at <http://localhost:4000>.

Writing a new draft
---
- Start in a draft mode: `bundle exec jekyll draft "My new draft"`
- `bundle exec jekyll publish _drafts/my-new-draft.md`
- or specify a specific date on which to publish it: `bundle exec jekyll publish _drafts/my-new-draft.md --date 2014-01-24`

Writing a new page or post directly
---
- `bundle exec jekyll page "My New Page"`
- `bundle exec jekyll post "My New Post"`

Configuration
-----

The main settings happen in side of the _config.yml file:

### Site

Main settings for the site

* **title**: name of your site
* **description**: description of your site
* **logo**: small logo for the site (300x * 300x)
* **cover**: large background image on the index page

* **name**: name site owner
* **email**: mail address of the site owner
* **author**: author name
* **author_image**: small image of author (300x * 300px)
* **disqus**: add a disqus forum for your post

### Social

The template allows to add all major social platforms to your site.
Fill the the form for each platform. If you leave the share_* entries empty, the sharing buttons below a post are not shown.  If you leave the **url** and **desc** empty the icons are not shown on the index page, but the share icons on the article pages remains untouched (Thanks to [Phil](https://github.com/philsturgeon))

* **icon**:	name of social platform (must match a name of [font-awsome](http://fortawesome.github.io/Font-Awesome/) icon set )
* **url**:	url of your account
* **desc**: slogan of the platform
* **share_url**: share url
* **share_title**: first part of url for the title
* **share_link**: second part of the share url for the link to the post

The Liquid template engine will magical combine the different parts to a share url.

```
http://twitter.com/share?text=post_title&amp;url=post_url
````

See [_config.yml](https://github.com/dirkfabisch/mediator/blob/master/_config.yml) for more examples.

Licensing
---------

[MIT](https://github.com/dirkfabisch/mediator/blob/master/LICENCE) with no added caveats, so feel free to use this on your site without linking back to me or using a disclaimer or anything silly like that.
