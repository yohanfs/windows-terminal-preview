README Windows Terminal Preview
=================================================================================

.. contents:: **Daftar Isi**

Set Default Shell
---------------------------------------------------------------------------------

click dropdown menu di terminal > Settings > Startup > Default profile


Custom Font dan Theme
---------------------------------------------------------------------------------

buka defaults.json, navigasikan ke:

::

        "profiles":
        {
                "default": {},
                "list":
                [
                        {
                                "colorScheme": "Cobalt2",
                                "fontSize": 9,
                                ....
                                ....
                        }

Profile **Cobalt2** didefinisikan di bagian schemes. Contohnya adalah:

::

        {
            "background": "#193549",
            "black": "#000000",
            "blue": "#1478DB",
            "brightBlack": "#808080",
            "brightBlue": "#1478DB",
            "brightCyan": "#00FFFF",
            "brightGreen": "#33FF00",
            "brightPurple": "#CC00FF",
            "brightRed": "#FF0000",
            "brightWhite": "#FFFFFF",
            "brightYellow": "#FFFF00",
            "cursorColor": "#FFFFFF",
            "cyan": "#00C5C7",
            "foreground": "#C7C7C7",
            "green": "#3AD900",
            "name": "Cobalt2",
            "purple": "#FF2C70",
            "red": "#FF2600",
            "selectionBackground": "#FFFFFF",
            "white": "#C7C7C7",
            "yellow": "#FFC600"
        },


Starting Directory
---------------------------------------------------------------------------------

*Starting directory* adalah direktori saat Windows Terminal Preview dibuka. 
*Starting directory* ini dapat di-set dengan menambahkan variable pada bagian list profile, sbb:

::

        {
                "colorScheme": "Cobalt2",
                "startingDirectory": "//wsl$/Ubuntu-20.04/home/username/"
        }
