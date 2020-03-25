# News

<div style="background: #fff3cd; padding: 1em; border-radius: 1em; text-align: left; font-weight: normal;">
	<b>Note</b>: This section assumes that you are already familiar with the <a href="/#/cms?id=content-management-system">Content Management System</a>
</div>

Managing news items on the site is easy. Every page on a GoBlender site is managed the same way.

Note that for the purposes of this guide, we draw a distinction between **pages**, **blog posts**, **news items**, and **calendar events**.
Although most of the functions used to manage content are the same, there are a few differences to be found among these four kinds of content.

Whenever you create an new blog post or edit an existing one, the screen will change to provide you with the tools necessary to do so. As we
saw in the [Content Management System](/#/content-management-system) section, you get a **Content Strip** along the left, and some **buttons**
(save, cancel, etc.)along the bottom. You will also notice a new button along the right hand side of the screen: a light grey box with a "<" symbol.

If you click on this button, called the **Edit Panel**, a pane will slide out from the right, revealing the basic news item details. Here is where you can
do the following:

## Set the news item name

The news item name can be whatever you wish, but is limited to 255 characters in length. Whatever you type here will be converted to a web-friendly
URL, using the following logig:

1. Spaces are converted to dashes
2. Special characters are removed
3. Everthing is converted to lower case

This, if you were to name your news item "Company ABC develops a new product: The Miracle Toaster", the automatically generated URL for the news item would be
`/news-item/company-abc-develops-a-new-product-the-miracle-toaster`. Note that all news items start with `/news-item`, and that this is added automatically.
You should not make that part of the title.

### Duplicate news item names

Sometimes you may give two or more news items the same name, either on purpose or inadvertently. In that case, the generated URL for the news item will have a number appended to it, so that there are no duplicate URLs on the site. For example, if you create two news items named "About", the first would have the URL of
`/news-item/about`, and the second would be given `/news-item/about-1`. This is an automatic process.

### Changing the URL of a news item

Typically, you don't want the URL of a page to change, ever. Thus, once a page is saved, its URL becomes immutable. For example, if you name a news item "What's New?" and then save it, its URL will be `/news-item/whats-new`. If you then edit the news item and change the name to `What's new today?`, the **URL wil not change**. If you wish to change the URL of the news item, you must copy its content, create a new news item, paste the content in, and give the news item a new name. You can then safely delete the old news item.

## Preview Image

Just below the title section of the **Edit Panel** you'll see a light grey square, and below that is a button labelled **Preview Image**. This allows you to specify what preview image you would like to use for the news item. The image is used on the `/news` page of the site, where news items are listed.

In order to specify a specific preview image, click the button, browse for the image, and upload it. It will auotmatically be converted to the proper
size for you.

## Preview Text

Just as you can specify what image is used on the `/news` page for previewing a post, you can also specify the preview text. If this is left empty,
the first few hundred characters of the news item will be used instead. Just click on the button to enter or modify the preview text.

## Meta Keywords

Meta keywords are hidden tags which appear in the `<head>` section of a web page. They are largely ignored by search engines these days, but
if you wish, you can enter a comma-separated list of keywords related to the page content.

If you set the meta tags, save the page, and then view source on your page, somewhere near the top you'll see a tag like this:

```html
<meta name="keywords" content="goblender, verilion, cms">
```

## Meta Description

The meta description is a hidden html tag which appears in the `<head>` section of a web page. If you wish, you can enter a brief description of your
page in this section. Search engines will sometimes, but not always, use this section when previewing your page in search results.

If you set the meta description, save the page, and then view source on your page, somewhere near the top you'll see a tag like this:

```html
<meta name="description" content="The official site for GoBlender, a content management system developed by Verilion Inc.">
```

You will also see tags like this:

```html
<meta property="og:title" content="GoBlender">
<meta property="og:description" content="The official site for GoBlender, a content management system developed by Verilion Inc.">
```

These are [Open Graph](https://ogp.me/) tags, which are used by many popular social media sites. As you can see, the title is taken from the **Page Title** section of
the page's **Edit Panel**, and the description is taken from **Meta Description**.


## News Date

Set the date for your news item by clicking on this field and choosing a date from the calendar.

<div style="background: #fff3cd; padding: 1em; border-radius: 1em; text-align: left; font-weight: normal;">
	<b>Note</b>: If you set the date in the future, the news item will not show up until that date!
</div>



## News Status

Almost any page on the site can be set to Active or Inactive, except for the home page, which must, for obvious reasons, always be active.

If a page is set to inactive and a visitor to the site tries to access it (by clicking on a bookmark, a search engine result, or just guessing the URL),
they will not be able to do so.

However, if a user is logged in, and has the rights to edit pages, he or she will be able to access the page. A warning notice will be displayed at the
top of the page, alerting you to the fact that the page is currently set to inactive.


## Access Level

Almost any page on the site can be given an access level, except for the home page, which must, for obvious reasons, always be accessible to the public.

There are three possible access levels:

1. Public - the post can be accessed by anyone
2. Account Required - the post can only be accessed by users who have an acccount, and are currently logged in
3. Administrators Only - only logged in users who are site administrators can see the post


## Menu Settings

Menu settings allows you to manage the way that the top navigation menu appears **for a specific page**.

Sometimes you may wish to have an image at the top of the screen that goes right up to the top, with no menu bar obscuring it. You can do so
by accessing the menu settings dialog by clicking on the **Menu Settings** button.  There are only two options to set:

1. Menu Text: this can be dark or light.
2. Menu Type: this can be normal (the default for your site, usually a light background), or Transparent, which makes the menubar background transparent.

So, if have a dark image at the top of the page (or a section with a dark background color), and you want the menu to blend into the top of the page,
you can set the menu to transparent, and the menu text to dark.

<div style="background: #ffcccb; padding: 1em; border-radius: 1em; text-align: left; font-weight: normal;">
	<b>Warning</b>: If you inadvertently set the menu text to the same (or a similar) color as the background of the page, it will look a lot like
	your menu has disappared. It hasn't. Roll your mouse around the top of the page and you will discover that it is still there, even though
	you cannot see it. Just edit the page again and change the menu text from light to dark (or vice versa) and the menu will appear again.
</div>


## Sharing Image

Sharing a page on social media is easy enough, but sometimes social media sites will not choose the image you want as a preview when the page is shared.
By clicking on the **Sharing Image** button, you can specify what image will be used when your page is shared on social media. The image must be at least
1200 pixels wide and 1080 pixels tall. It will be convereted to the correct dimensions for sharing on major social media sites.

If you set the sharing image, save the page, and then view source on your page, somewhere near the top you'll see tags like the ones below:

```html
<meta property="og:image" content="http://localhost:4000/static/site-content/page-uploads/7/fb.jpg">
<meta name="twitter:image" content="http://localhost:4000/static/site-content/page-uploads/7/twitter.jpg">
```

These tags are generated from the sharing imagen chosen for the page, converted to formats approrpriate for social media sites.

## Javascript and CSS

At the very bottom of the **Edit Panel** are two icons: one for JavaScript, and one of CSS. You can enter **page specific** JS or CSS here. Note that
the JS and CSS will only be applied to the current page.
