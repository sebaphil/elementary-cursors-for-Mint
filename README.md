elementary Cursor Theme redesigned for Linux Mint
=================================================
### Preview

[![Preview](https://github.com/AlessandroBusolin/elementary-cursors-for-Mint/blob/master/preview/elementary.png)](#features)

A cursor theme for elementary OS redesigned for Linux Mint

These cursors are free artwork; you can redistribute them and/or modify them under the terms of the [GNU General Public License version 3](http://www.gnu.org/licenses/gpl.txt).

### Installing 

Copy the 'elementary' folder into '/usr/share/icons', then set your cursor theme using your favourite tool or:

    gsettings set org.gnome.desktop.interface cursor-theme 'elementary'

But to make a system-wide change run the following:

    sudo update-alternatives --install /usr/share/icons/default/index.theme x-cursor-theme /usr/share/icons/elementary/cursor.theme 13
    sudo update-alternatives --set x-cursor-theme /usr/share/icons/elementary/cursor.theme

Then log out and back in for the changes to take effect.

For manual installation, you may have to change the copied files' permissions (to 755) after copying in order to use the theme.

### Using the Source

There are scripts to simplify the rendering process; to run them (and edit icons) you will need:

 * inkscape
 * python

To render the cursor theme from the [source plate](src/cursors/elementary.svg) you will need to run the render script in [src/cursors](src/cursors):
	
	cd src/cursors
    python renderpngs.py

Then make the theme by running the make script in the [src/cursors/pngs](src/cursors/pngs) folder:

	cd src/cursors/pngs
    bash make.sh

-----------

"elementary Cursor Theme" ridisegnato per Linux Mint
====================================================

Un tema per il cursore di elementary OS ridisegnato per Linux Mint

Questi cursori sono opere d'arte gratuite; li puoi redistribuire e/o modificare secondo i termini della [GNU General Public License version 3](http://www.gnu.org/licenses/gpl.txt).

### Installazione

Copia la cartella 'elementary' dentro '/usr/share/icons', quindi imposta il cursore usando il tuo programma/strumento preferito oppure:

    gsettings set org.gnome.desktop.interface cursor-theme 'elementary'

Ma per fare un cambiamento a tutti i livelli del sistema devi eseguire i seguenti comandi:

    sudo update-alternatives --install /usr/share/icons/default/index.theme x-cursor-theme /usr/share/icons/elementary/cursor.theme 13
    sudo update-alternatives --set x-cursor-theme /usr/share/icons/elementary/cursor.theme

Quindi esegui il log out per rendere effettivi i cambiamenti.

Per l'installazione manuale, potrebbe essere necessario che modifichi le autorizzazioni dei file copiati (a 755) dopo la copia, per poter utilizzare il tema.
