
# UTM Robotics Club Website

Based on janczizikow's [Sleek Jekyll theme](https://github.com/janczizikow/sleek)

## How to Use

### Website Configuration

The YAML file `_config.yml` contains all the basic configuration settings for the website.

Some important fields:

* `gcalendar_api_key`: Google Calendar API key
* `navigation`: Defines all navigation links
* `twitter_username`, `facebook_username`, `instagram_username`, `slack_link` define the links for the array of social buttons shown at the bottom of pages.

### Calendar

The calendar is fully managed by Google Calendar. Any changes made to the corresponding Google Calendar will be reflected on the website calendar.

### Posts/Events

Navigate to the `_posts` folder from the root directory.

#### Managing Posts

* Edit event: edit markdown file
* Remove event: remove markdown file
* Create event: create markdown file with the following filename format
	* `year-month-day-title-seperated-by-dashes.md`
	* An example filename would be `1999-01-01-some-title.md`

#### Post Format

For every post add a header with the following format:
```
---
layout: post			<- post refers to the layout type
title: "Sample Title"		<- title of post
time: "1-2 pm"			<- time of event
location: Someplace		<- location of event
featured-img: sample		<- image for post (optional)
categories: [a,b,c]		<- tags for post (optional)
color: rgb(200, 100, 100)	<- color for post (optional)
---
```
Note that `color` and `featured-img` are mutually exclusive.

#### Post images

To add images, upload `.jpg` pictures in the folder `assets/img/posts`.

Images with aspect ratio `16:9` display the best.

To link to a specific post, edit the `featured-img` attribute in the post header to the filename of the `.jpg` excluding the file extension.

Example: `sample.jpg -> sample`

### Pages

Navigate to the `_pages` folder from the root directory. To edit a page, edit the corresponding markdown file.

For every page add a header with the following format:
```
---
layout: page			<- page refers to the layout type
title: About			<- title of page
permalink: /about/		<- url endpoint
---
```
### Embedding Media, Links and Code Snippets

To add images, use the following format
* `![text to show on fail load]({{ site.url }}{{ site.baseurl }}/path-to-file-from-root)`

To embed YouTube videos, use the following format
* `{% include youtube.html link="https://www.youtube.com/embed/some-random-id" %}`

To add links, use the following format
* `[link text](actual-website-link)`

To add code snippets, begin with `` ```programming-language`` as the header, then write the code, and end with `` ``` `` as the footer.

### Editing Templates

To edit templates, edit the `.html` files found in the `_includes` or `_layouts` folder. The `.html` files support the Liquid template language.

### Styling

To add custom styles, edit the `.scss` files in the folder `_sass`. Jekyll will automatically compile the equivalent `.css` file for you.
