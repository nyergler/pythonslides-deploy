====================
Python Slides Deploy
====================

This repository contains the Ansible_ playbooks needed to deploy
`Python Slides`_ or `Read the Docs`_. The playbooks are based on
`django-ansible`_, itself based on Matthew Makai's `SF Django Meetup
examples`_.

Getting Started
---------------

This repository contains a Vagrantfile_, and defaults to targeting a
single Vagrant_ virtual machine as the web and database server. You
can get started by simply::

 $ vagrant up
 $ ansible-playbook -i hosts django-stack.yml

If you want to use these playbooks to deploy Read The Docs or other
Django applications, the ``group_vars/all`` file is a good place to
start.


.. _Ansible: http://ansible.com/
.. _`Python Slides`: https://github.com/nyergler/pythonslides
.. _`Read the Docs`: https://github.com/rtfd/readthedocs.org
.. _`django-anssible`: https://github.com/nyergler/django-ansible
.. _`SF Django Meetup examples`: https://github.com/makaimc/sf-django
.. _Vagrant: http://www.vagrantup.com/
.. _Vagrantfile: http://docs.vagrantup.com/v2/vagrantfile/
