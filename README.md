 git_templates
===============

Git templates are a feature that populates git repositories with a
template to start with. Typically this is used for populating useful
hooks.

These hooks are meant to be helpful to people developing for
OpenStack.

Installation
----------

Installation is pretty straight forward.

    git clone https://github.com/sdague/git_template
    git config --global init.templatedir /PATH/TO/git_template

    cd somedirectory
    git init


Note you can git init an existing git repository, and it will copy
over **new** template files. However if you already had an old version
of a template file, it will not be replaced.

Functionality
------------

- pre-commit
    - if .gitreview file exists, prevent committing to master branch
