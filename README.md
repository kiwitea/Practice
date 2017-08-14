# TODO

## Invalid theme
### Fatal Errors

(Must-fix to activate theme)
Replace {{pageUrl}} with {{page_url}}

The helper {{pageUrl}} was replaced with {{page_url}}.
Find more information about the {{page_url}} helper here.
Affected files:
    partials/pagination.hbs: Please remove or replace {{pageUrl}} from this template
Replace the {{image}} helper with {{img_url feature_image}} or {{img_url profile_image}}

The {{image}} helper was replaced with {{img_url}}.
Depending on the context of the {{img_url}} helper you would need to use e. g.

{{#post}}
    {{img_url feature_image}}
{{/post}}

to render the feature image of the blog post.
Find more information about the {{img_url}} helper here and read more about Ghost's usage of contexts here.
Affected files:
    partials/loop.hbs: Please remove or replace {{image}} from this template
    post.hbs: Please remove or replace {{image}} from this template
Replace the {{@blog.cover}} helper with {{@blog.cover_image}}

The cover attribute was replaced with cover_image.
Instead of {{@blog.cover}} you need to use {{@blog.cover_image}}.
See here.
Affected files:
    default.hbs: Please remove or replace {{@blog.cover}} from this template
Replace the {{#if image}} helper with {{#if feature_image}}, or {{#if profile_image}}

The image attribute was replaced with feature_image and profile_image.
Depending on the context you will need to replace it like this:

{{#author}}
    {{#if profile_image}}
        {{profile_image}}
    {{/if}}
{{/author}}

See the object attributes of author here.

{{#post}}
    {{#if feature_image}}
        {{feature_image}}
    {{/if}}
{{/post}}

See the object attributes of post here.

{{#tag}}
    {{#if feature_image}}
        {{feature_image}}
    {{/if}}
{{/tag}}

See the object attributes of tags here.
Affected files:
    partials/loop.hbs: Please remove or replace {{#if image}} from this template
    post.hbs: Please remove or replace {{#if image}} from this template




# Practice

![Practice Theme Demo](https://github.com/Dennis-Mayk/Practice/blob/master/preview.gif)
<br>
A clean timeline theme for the Ghost CMS.
This theme has been build from the ground up with a focus on only the most essential elements to keep the user experience smooth and fast.

## Installation
Just download an instance of <b>Practice</b> to your ghost's theme folder (you eventually will need to restart ghost).

Please select an even number of posts per page in the pagination settings in your ghost dashboard for perfect pagination performance.

## Release notice
<code>
08.01.2017 Fixed tag page error + updated stylesheet and preview gif
</code><br>
<code>
05.01.2017 Fix ghost pro errors, make more generic for others to use - by <a href="https://github.com/xdumaine">xdumaine</a>
</code><br>
<code>
30.07.2016 Practice now uses <a href="https://github.com/infinite-scroll/infinite-scroll">infinite scroll</a> for pagination v1.4 
</code><br>
<code>
27.07.2016 Changed typography, navigation and allows now background images v1.3 
</code><br>
<code>
10.07.2016 Added footer section for credits v.1.2
</code><br>
<code>
06.07.2016 PageSpeed optimized v.1.1
</code><br>
<code>
01.07.2016 Release of Practice v.1.0
</code>

## Contributors - many thanks to you!
[xdumaine](https://github.com/xdumaine) | [Br3nda](https://github.com/Br3nda)
