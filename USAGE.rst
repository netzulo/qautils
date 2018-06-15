USAGE GUIDE
===========


Files
-----

Have classes for this down package: ``qautils.files``

- Methods for **package**
  + method **path_format** : ``TODO: fill up section``
  + method **read_file** : ``TODO: fill up section``
  + method **read** : ``TODO: fill up section``
  + method **settings** : ``TODO: fill up section``


.. code:: python


    from qautils.files import settings


    # file_path = './' by default
    SETTINGS = settings(
        file_path="/home/user/config/dir/",
        file_name="settings.json"
    )
    KEY_TO_CHECK = "some_json_key_name"


    try:
        print(SETTINGS[KEY_TO_CHECK])
    except Exception as err:
        print("ERROR: {}".format(err))
    finally:
        bot.close()
