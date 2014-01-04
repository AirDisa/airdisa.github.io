airdisa.github.io
=================

Stable: 0.6.0
-------------

@AirDisa Jekyll Website for GitHub.io

Changelog
---------

* 2013-01-04 Integrated LSI build
* 2013-01-02 Implemented .gitignore
* 2013-12-31 Implemented related\_posts LSI
* 2013-12-30 Implemented \_drafts
* 2013-12-29 Implemented pagination
* 2013-12-24 Initial commit

Code is FOSS unless otherwise cited. Content is protected.

What's inside?
--------------

* Jekyll
* Redcarpet
* YAML
* JSON
* Ruby
* Latent Semantic Indexing

Directory Structure
------------------

    _drafts/
      .gitignore      # Drafts staged for preview, git ignored

    _layouts/         
      default.html    # Default layout template
      post.html       # Post layout template

    _posts/         
      2013-12-24.md   # Initial post, title removed here for brevity
      2014-01-01.md   # Post for 2014, initially created as a draft
      etc.

    _site/             
      css/            # Generated CSS files by Jekyll build
      github/         # Generated topic directory by Jekyll build
      jekyll/         # Generated topic directory by Jekyll build       
      pg/             # Pagination folder, organized into page number directories
      wordpress/      # Generated topic directory by Jekyll build              

    css/
      main.css        # Sitewide CSS
      syntax.css      # Snippet highlight Pygments markdown CSS

    _config.yml       # Jekyll options
    github.html       # Github topic category index
    index.html        # Index, now paginated
    jekyll.html       # Jekyll topic category index
    LICENSE           # Copyrighted content, otherwise FOSS
    wordpress.html    # Wordpress topic category index


Install Jekyll
--------------

#### Use sudo when needed

~ $ gem install jekyll

~ $ jekyll new project\_directory

~ $ cd project\_directory

~ $ vim # => or emacs


Install JSON
------------

~ $ gem install json


Jekyll Build
------------

~ $ jekyll build # => Build website files

~ $ jekyll build --lsi # => Build website files, with latent semantic indexing

Run the server

~ $ jekyll server # => Browse http://localhost:3000

~ $ jekyll server --drafts # => Preview option, includes drafts


As hosted by GitHub Pages
-------------------

Browse: [http://airdisa.github.io](http://airdisa.github.io)

Copyright 2013-2014 Disa Johnson. All rights reserved.
