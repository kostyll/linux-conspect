
File group encoding convertion
------------------------------
Simple case:
to convert encoding in some directory of some file group you may use the following command

.. code-block:: bash

    for file in *.php; do
         iconv -f windows-1251 -t utf-8 "$file" -o "${file%}";
    done

