# HTML

## Elements 

An element consists of a start tag (<), some content, and an end tag (>).

### Tags

Tags are labels you use to mark the beginning and end of an element. 

Two types of tags:

	- Opening (i.e. <html>)
	- Closing (i.e. </html>)

Some tags do not require a closing tag in order to be complete. These tags lead to what are called "void elements".

Writing tags lowercase is the standard, and good form

Several elements can be used in sequence, as long as they are properly nested. Avoid overlap in the element tags, or else trouble can occur


#### Tags List:

Tag					Use				
_em /em_			Italicize contents.
_h{1-6} /h{1-6}_	Headers, 1 being the largest and 6 being the smallest.
_br_				Creates an extra line between the last piece of text and the following text.
_html /html_		Lets the browser know the language of the HTML document you are using.
_head /head_		Provides information about your HTML document
_body /body_		Denotes where you should place the content of the HTML document
_title /title_		Used within the head tags to denote what title should be displayed in the tab in your web browser
_p /p_				Separates out a text paragraph
_strong /strong_	Used to make text bold and emphasized
_small /small_		Used to shrink text a bit, to de-emphasize it in a way
_hr_				Draws a horizontal line on the page. If used in the middle of text, it will add a new line, then the horizontal line, then continue the text on the next line
_ul /ul_			Creates an unordered list. Must be combined with _li_
_ol /ol_			Creates an ordered list. Must be combined with _li_
_li /li_			Denotes a list item. Used within either _ul_ or _ol_ tags
_a /a_				Stands for anchor, used for links
_img_				Allows the insertion of an image into your document
_table /table_		Creates a table with the values within the tags.
_tr /tr_			Creates a row of data within the _table_. This may contain many individual elements within its tags.
_td /td_			Creates an individual cell of data within a row in a _table_
_th /th_			Creates a column heading in a _tr_ of a _table_. Used instead of _td_
_style /style_		Used within _head_ to add style generally to the entire document. (<style type="text/css">)



### Attributes

Attributes can be added to specific elements. These attributes are written within the first tag of the element, and provide extra information to the browser.

Some attributes are only used with certain elements. But the attributes associated with certain tags are logical, and make sense.

#### Attribute List:
Attribute			Use
_title_				Added to headers and other open tags. Adds a short description of the content of that element when you hover the mouse over it. Can be used with images as well.
_style_				Can be used to add background colors and other style fixes. If used in the _body_ tag, changes for the whole page. Otherwise, changes for the scope of the element
	- background-color: Used to change the background color of an element
_href_				Stands for "hypertext reference". Specifies where a link leads to. A link can be: a website, a file in your directory, a subfolder, an email address, etc.
_id_				Used to allow links within a page. It must start with a letter, and is referenced with #
_mailto_			Used within _href_ to link to an email address. EXAMPLE: href="mailto:nobody@html.net"
_src_				Used within _img_ to designate the location of the image in the directory tree, or the address where the image is.
_alt_				Used within img to give an alternate description if for some reason the image cannot be displayed.
_width_ + _height_	Used within _img_ to specify the width and height of the image. The values used are in pixels. Does not actually change the actual file size. NOTE: After the number, a px is included
_border_			Used within _table_ to add a border to a table is set equal to 1. (border="1")
_colspan_			Used within _td_ to specify how many columns the cell should span.
_rowspan_			Used within _td_ to specify how many rows the cell should span


### Links

Links in HTML are super easy. By combining the _a_ tag and the _href_ attribute, you can basically link to anything you can fit in the element.

EXAMPLE: <a href="http://www.html.net/">This is an example link</a>


### Images

Images are super easy to input into an HTML file. The _img_ tag is encase in the _figure /figure_ tags to denote that there's an image there. Images can also be used as links, by enclosing them in _a /a_ tags within the _figure /figure_ tags


### Tables

Tables in HTML use a lot of tags, but are quite logical.
