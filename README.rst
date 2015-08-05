Mobs
----

My own backup strategy, enabled by Ansible.

--------------
Requirements
--------------

- ansible_
- duplicity_
- gpg_

-------------
Quick Start
-------------

To list your gpg keys, run: 

::

    gpg --list-keys

To install, run:

::

    ansible-playbook site.yml --extra-vars "user=yourlocaluser gpg_key=yourgpgkey backup_target=yourbackuptarget"


.. _ansible: http://www.ansible.com/
.. _duplicity: http://www.nongnu.org/duplicity/
.. _gpg: http://www.gnu.org/software/gnupg/
