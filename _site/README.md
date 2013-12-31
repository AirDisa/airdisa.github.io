airdisa.github.io
=================

Stable: 0.3.0
-------------

@AirDisa Jekyll Website for GitHub.io

Changelog
---------

* 2013-12-30 Implemented \_drafts
* 2013-12-29 Added pagination
* 2013-12-24 Initial commit

Code is FOSS unless otherwise cited. Content is protected.

What's inside?
--------------

* Ruby
* Jekyll
* Redcarpet
* YAML
* JSON

Directory Structure
------------------

    _layouts/         
      default.html    # Default layout template
      post.html       # Post layout template

    _posts/         
      2013-12-24.md   # Initial post, title removed here for brevity
      2014-01-01.md   # Post for 2014, initially created as a draft

    _site/             
      css/            # Generated CSS files by Jekyll build
      github/         # Generated topic directory by Jekyll build
      jekyll/         # Generated topic directory by Jekyll build       
      pg/             # Pagination folder, organized into page number directories
      wordpress/      # Generated topic directory by Jekyll build              

    css/
      main.css        # Sitewide CSS
      syntax.css      # Code snippet highlight Pygments markdown CSS

    _config.yml       # Jekyll options
    github.html       # Github topic category index
    index.html        # Index, now paginated
    jekyll.html       # Jekyll topic category index
    LICENSE           # Copyright status of FOSS
    wordpress.html    # Wordpress topic category index


Install Jekyll
--------------

~ $ gem install jekyll
~ $ jekyll new gh-pages
~ $ cd gh-pages
~ $ /gh-pages
~ $ jekyll serve      # => Now browse to http://localhost:3000

* Port: 3000 option in \_config as it is the only port I allow

Jekyll Build
------------

~ $ jekyll build      # Regenerate website flat files, use --drafts option to add those

Run the server

~ $ jekyll server     # Find excellent server options in documentation

As hosted by GitHub

Visit: [http://airdisa.github.io](http://airdisa.github.io)

Copyright 2013-2014 Disa Johnson. All rights reserved.
