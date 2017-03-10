# www.alexsommer.io

* * *
#### tl;dr: **this is a website I made**

* * *
##### Stack
* * *
* DNS host: godaddy.com
* site hosting: GitHub servers (probably Linux or RedHat)
* blog framework: Jekyll
* 1 CSS stylesheet and 2 templates [`styles.css`, `blog.html`, `default.html`]

If you're unfamiliar with [Jekyll](http://jekylllrb.com), it is an awesome blog tool that lets you use html injections and templating to write blog posts and share media incredibly easy. It compiles your project into a `_site/` directory that is served publically. It's a very lightweight framework that seeks to not make any large assumptions about your site's workflow and setup, and thus permits a lot of flexibility. It also is open-sourced and has a really responsive and kind community under the MIT License.

Here's a bash tree of my project's directory structure:
```markdown
├── CNAME
├── Gemfile
├── Gemfile.lock
├── README.md
├── _config.yml
├── _includes
│   ├── google-analytics.html
│   ├── header.html
│   ├── page-bottom.html
│   └── page-top.html
├── _layouts
│   ├── blog.html
│   └── default.html
├── _posts
│   ├── 2010-11-08-first-post.md
│   ├── 2013-12-19-religious-discourse-in-the-public-sphere.md
│   └── 2016-07-09-uc-berkeley-antisemitism.md
├── assets
│   ├── css
│   │   └── styles.css
│   └── img
│       ├── favicon.ico
│       └── resume_2015.jpg
├── blog
│   └── index.html
├── index.html
└── resume
    └── index.html
```

* * *
##### Lessons Learned
* * *
I was curious how hard it would initially be to just run a static site serving HTML+CSS, but I quickly realized that having to duplicate exactly identical code is never a good reason because it just asks to be inconsistent. If you do something as simple as change the ordering of button links at the top of the page, you're going to have to find every view that presents that information and change a bunch of static text. Instead, if you are running a service such as Jekyll, you can write `{% include something.html %}` and it will liquidly inject the HTML for you, reducing the diffs you need to make (and the ones you will inevitably forget). There are a bunch of other features also like pre-formatted variables and views as templates along with auto-formatted URLs using permalink customization.

* * *
##### Next Steps
* * *
I'm just starting out I'll hopefully write about future things I do, but I don't have that many desires other than a simple site that can serve my writing content. Because this is no longer being hosted on godaddy.com, I can't SSH or SFTP into the box and mess around with server-side scripting or databases. godaddy still has that, but it was also more robust than I needed (and also more pricey than $0 to host).

* * *




