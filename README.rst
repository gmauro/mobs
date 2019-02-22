Mobs
====

My own backup strategy, enabled by Ansible.

--------------
Requirements
--------------

- ansible_
- duplicity_
- gpg_

---------------
Quick Start
---------------

Generate an OpenPGP key setting a passphrase (see this howto_):

::

    gpg --gen-key

To list your gpg keys, digit:

::

    gpg --list-keys

To install Mobs, edit defaults/main.yml accordingly to your setup, then digit:

::

    ansible-playbook site.yml -e "@defaults/main.yml"


.. _ansible: http://www.ansible.com/
.. _duplicity: http://www.nongnu.org/duplicity/
.. _gpg: http://www.gnu.org/software/gnupg/
.. _howto: https://help.ubuntu.com/community/GnuPrivacyGuardHowto
