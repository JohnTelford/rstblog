Build a Sphinx Blog
===================

.. post:: Dec 7, 2020
   :tags:
   :category:

.. Note:: 
   
   - Work in Progress

*Home page* :ref:`Tech Talk Blog`

Synopsis
--------

This post is about creating and deploying this blog, :ref:`Tech Talk Blog`

Since the early days of the web, I have been building  blogs and web sites from scratch or using the  technology du jour. 

My technology preferences are :ref:`vsCode` , :ref:`Sphinx`, :ref:`reStructuredText`, :ref:`Netlify`, and GitHub.   

I use :ref:`vsCode` as Central Command and Control for managing this blog. I edit source files with a live preview edit window showing rendered file changes. Compiling  the web site, uploading  to Netlify for  deployment to the web, takes less than 30 seconds. Repo changes are pushed  to GitHub using vsCode.

I think his is the best and faster web development technology I have cobbled.


Sphinx
------

This web site is built using :ref:`Sphinx`  It uses :ref:`reStructuredText`  as its markup language, and many of its strengths come from the power and straightforwardness of reStructuredText and its parsing and translating using the Docutils [#]_ suit,  

Sphinx [#]_ is web site generator for creating web sites and other types of documentation. It requires using Markdown [#]_, or :ref:`reStructuredText` which is  a  user-friendly, plain text markup language,  for editing web site and other text material. 

-----

Sphinx [#]_ is the framework for building this site. It   requires  using :ref:`Markdown`  or :ref:`reStructuredText` for text material editing. My preference is reStructuredText.   

Most development time is spent editing web site text material. The VScode reStructuredText Extension [#]_ dramatically speeds up development  supports reStructuredText features:

    - Syntax highlighting quickly detects :ref:`reStructuredText` errors while typing or compiling, and may give hints about the problems
    - Frequent snippets of code can be quickly inserted
    - Section builder provides a quick way for setting section header levels
    - Live preview compiles source files in the background. Quickly invoking live preview while editing, shows how the edit will be displayed on the web


reStructuredText
----------------

:ref:`reStructuredText`  is a lightweight markup language that is used in static site generators like :ref:`Sphinx`. Sphinx requires using Markdown or reStructuredText for text material editing. This web site is an example of using reStructuredText and Sphinx. 

Sphinx contains robust tools for semantic markup, reusing content, and content filters for different kinds of outputs.

Compared to some other lightweight markup languages like Markdown, reStructuredText contains stronger semantic markup tools. Some writers also prefer reStructuredText because the markup standards are more well-defined compared to MarkDown

reStructuredText is an easy-to-read,  plaintext markup syntax and parser system. The  syntax is relative easy to read and can be translated to Markdown.

Regardless of the framework using a flavour of Markdown,  my experience is embedding HTML with Markdown was necessary every so ofter. Not so with reStructuredText.

A useful feature of Sphinx is one can see the reStructuredText used to create a web page by clicking on "Page source" in the lower right corner of a web page. I used this to speed up learning Sphinx. I think reStructuredText is easier to read than markdown.

It is useful for quickly creating simple web pages, and for standalone documents

"Structured Text" is probably a bit of a misnomer. It's more like "Relaxed Text" that uses certain consistent patterns. These patterns are interpreted by a HTML converter to produce "Very Structured Text" that can be used by a web browser

reStructuredText is the default plaintext markup language for Sphinx and many of its strengths come from the power and straightforwardness of reStructuredText and its parsing and translating suite, the Docutils [#]_

-----

My preference is using :ref:`reStructuredText` and :ref:`Sphinx` framework.   Its syntax is relative easy to read and can be translated to Markdown.



Blog
----

ABlog for Sphinx [#]_ is a Sphinx extension that converts any documentation or personal website project into a full-fledged blog 


vsCode
------

I use vsCode to edit and manage my Tech Talk John blog, with a live preview edit window to view rendered file changes.

It takes Sphinx 13 sec. to compile a 755 files / 89 MB blog directory structure, and Netlify CLI  6.5 sec to copy and deploy it to a CDN. I can edit files and within 20 seconds see the blog on the web.

This process speeds up my time proof reading and correcting errors. A wise tech writer once said to render writings in different media before publishing.


-----

Developers using  Visual Studio Code [#]_ as   Central Command and Control   enables  developing, managing,  controlling, and deploying web sites. VScode, is a lightweight open source code editor that runs on local development computers,  and is available for Linux, macOS, and Windows. It may be the best text editor in years

-----

**blog**


-----

Netlify
-------

Netlify [#]_ is a popular Application Delivery Network (ADN). It provides continuous web deployment. 

- One Way is when Netlify is notified of a commit to a shared GitHub repository that has been configured, Netlify builds the web sites from the  shared repository and deploys the web worldwide to every major cloud provider.

- Another way is using the Netlify CLI Command [#]_ program running on the local development computer,  Netlify can deploy draft previews of live web sites.


Frequently viewing drafts of the entire web site on the web helps.

I prefer using Netlify CLI Command. I still commit to a GitHub repository to help me keep my sanity. I have configure Netlify not to build the web site after a repository commit.




Deploying web site draft preview:
::

    # Compile reStructuredText to HTML
    ablog build
    # Deploy web site draft preview 
    netlify deploy 
    # Click on the Website Draft  URL


If the draft preview looks good, deploy production using the ``--prod`` flag
::

    # Compile reStructuredText to HTML
    ablog build
    # Deploy production web site
    netlify deploy --prod
    # Click on the Website URL



-----

.. rubric:: Footnotes:

.. [#]  Sphinx : https://www.sphinx-doc.org/en/master/index.html

.. [#] Markdown Syntax Guide: https://daringfireball.net/projects/markdown/syntax


.. [#] reStructuredText: https://en.wikipedia.org/wiki/ReStructuredText

.. [#] Docutils: http://docutils.sourceforge.net

.. [#] ABlog for Sphinx: https://ablog.readthedocs.io

.. [#] Get started with Netlify CLI: https://docs.netlify.com/cli/get-started/#run-builds-locally
-----

*Home page* :ref:`Tech Talk Blog`
