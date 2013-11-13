# Oops
You probably want https://git.gnome.org/browse/gnome-epub-thumbnailer instead; it does mobi files, too! Of course, I discovered that this existed a couple of hours after I wrote this one.

# What?
mobi-thumbnailer is a simple script that tries to find a cover into a Mobipocket ebook file and creates a thumbnail for it.

# Why?
To show off the covers of my Kindle ebooks.

# How to install?
Make sure mobi-thumbnailer is executable

    chmod +x mobi-thumbnailer

Copy mobi-thumbnailer to /usr/bin

    sudo cp mobi-thumbnailer /usr/bin

# If you are running gnome2
Copy mobi-thumbnailer.schemas to /usr/share/gconf/schemas/

    sudo cp mobi-thumbnailer.schemas /usr/share/gconf/schemas/

Install the schema

    gconftool-2 --install-schema-file /usr/share/gconf/schemas/epub-thumbnailer.schemas

# If you are running gnome3 (aka gnome-shell)
Copy mobi.thumbnailer to /usr/share/thumbnailers

    sudo cp mobi.thumbnailer /usr/share/thumbnailers/

# To complete the installation
Restart nautilus

    nautilus -q && nautilus

# Acknowledgments
- [Marcelo Lira](https://github.com/setanta): Created epub-thumbnailer, which I based this on
- [Renato Ramonda](https://github.com/renatoram): Added gnome3 thumbnailer support
