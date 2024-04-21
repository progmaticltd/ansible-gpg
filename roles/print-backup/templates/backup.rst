GPG key backup {{ gnupg.name }}
=========================================

Certify key
-----------

paper version
^^^^^^^^^^^^^

::

{% for line in certify_key_paper_lines %}
  {{ line }}
{% endfor %}

Passphrase
^^^^^^^^^^

::

  {{ certify_key_passphrase }}

QR Code
^^^^^^^

.. image:: ./certify-key-qr.png
   :width: 60%

Sub keys
--------

paper version
^^^^^^^^^^^^^

::

{% for line in subkeys_paper_lines %}
  {{ line }}
{% endfor %}

Passphrase
^^^^^^^^^^

QR Code
^^^^^^^

.. image:: ./subkeys-qr.png
   :width: 60%


LUKS passphrase
---------------

::

  {{ luks_passphrase }}
