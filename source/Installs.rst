.. _post: Sep 20, 2020

Creating a rstBlog
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

Transfer Blog
-------------

rusync build/html /Volumes/Dev/rstJohn/build/html/rstBlog

Deploying to Netlify
--------------------




