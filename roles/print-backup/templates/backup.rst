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

Acrostic: ``{{ certify_key_acrostic }}``

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

QR Code
^^^^^^^

.. image:: ./subkeys-qr.png
   :width: 60%

{% if luks_passphrase is defined %}
LUKS passphrase
---------------

::

  {{ luks_passphrase }}

{% endif %}
