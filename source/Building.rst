
Building a rstBlog
==================

Sep 20, 2020 11-06 AM

Some assembly is required to create a rstBlog 

Shell
-----

Mac Shell Install Commands::

    cd /Volumes/Dev/rs/
    git clone https://github.com/JohnTelford/rstblog.git
    cd rstblog
    brew install sphinx
    sphinx-quickstart
    pip install -U ablog

Deploying to Netlify
--------------------

This is Cliff notes::

    make a git repo
    connect netlify to repo
    download netlify CLI
    go to blog root
    netlify init
    netlify deploy --prod



