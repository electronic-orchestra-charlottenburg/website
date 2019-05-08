=============================================
Electronic Orchestra Charlottenburg (website)
=============================================

This is the source code for the static website of the Electronic Orchestra
Charlottenburg.
|nikola| is used to generate the static content from this source code
repository. Have a look at its |handbook| for more information.

The website is configured in `conf.py`. Its pages are generated from |rst|
files in the pages directory and its news from |rst| files in the posts
directory.
The photo galleries are created from files in directory structures under the
galleries directory and anything placed in the files directory will be copied
to the root of the website.

Currently a standard theme is used with slight modifications applied from
`files/assets/css/custom.css`

Installing nikola
#################

To install nikola, either use your distributions package manager:

  .. code:: bash

    # Arch Linux example
    pacman -S nikola

    # Ubuntu/Debian example
    apt-get install nikola

Alternatively, you can install it via pip3:

  .. code:: bash

    pip3 install --user nikola

If installing through pip, make sure to add *~/.local/bin* to your **$PATH**
afterwards (if that's not already the case):

  .. code:: bash

    # ~/.bash_profile
    export PATH="${HOME}/.local/bin:${PATH}"


Working with the code base
##########################

Build the website:

  .. code:: bash

    nikola build

To run the website locally:

  .. code:: bash

    nikola serve

To deploy the website to its webserver destination:

  .. code:: bash

    nikola deploy

| You need to have a valid ssh key on the remote host machine.
| Please make sure to add the latest deploy and push it to the repository:

  .. code:: bash

    git add state_data.json
    git commit -m "state_data.json: Deployed website."
    git push


.. |nikola| raw:: html

  <a href="https://getnikola.com/" target="_blank">Nikola</a>

.. |handbook| raw:: html

  <a href="https://getnikola.com/handbook.html" target="_blank">handbook</a>

.. |rst| raw:: html

  <a href="http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html" target="_blank">reStructuredText</a>

