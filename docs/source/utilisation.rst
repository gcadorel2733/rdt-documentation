Utilisation de Home Assistant
=====

.. _installation:

Redémarrage de Home Assistant
--------
Pour redémarrer Home Assistant :
   1. Cliquer sur **Paramètres**
            .. image:: images/parametres.png
               :width: 150
               :align: center
   2. Choisir **Système**
         .. image:: images/systeme.png
            :width: 500
            :align: center
   3. Cliquer en haut à droite sur le bouton.
            .. image:: images/reboot.png
               :width: 50
               :align: center

Documentation de cartes personnalisés
--------

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

