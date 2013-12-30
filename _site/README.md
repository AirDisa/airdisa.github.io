airdisa.github.io
=================

Stable: 0.2.0
-------------

@AirDisa GitHub Jekyll Website

Changelog
---------

* Added pagination 2013-12-29
* Initial commit 2013-12-24

Code is FOSS unless otherwise cited. Content is protected.

What's inside?
--------------

* Jekyll
* Redcarpet
* YAML

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
    ~ $ jekyll new my-awesome-site
    ~ $ cd my-awesome-site
    ~/my-awesome-site $ jekyll serve # => Now browse to http://localhost:4000

* Requires Ruby

Jekyll Build
------------

    ~ $ jekyll build    # Regenerate website flat files

Run the server

    ~ $ jekyll server   # Local server option

As hosted by GitHub

Visit: [http://airdisa.github.io](http://airdisa.github.io)

Copyright 2013-2014 Disa Johnson. All rights reserved.
