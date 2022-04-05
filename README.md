My rather opinionated GTK3 fork. Standard GTK is opinionated too, only their
opinions are wrong. Features include:

- Everything from [gtk3-classic](https://github.com/lah7/gtk3-classic), except
  the pointless change from Evince to Atril.
- CSDs are more thoroughly trounced. Since Classic's tweaks didn't work for me,
  I just gutted a couple of related functions entirely. As a result, CSDs are
  unequivocally disabled, with no flag to enable.
- File chooser sidebar is cleaned up, with no silly English terms cluttering
  the place.
- If [kodoku](https://github.com/Kyuuhachi/kodoku) is loaded, loads
  `$KODOKU_HOME/gtk/.config/gtk-3.0/settings.ini` as well as the standard paths
- If kodoku is loaded, file choosers consider `$USER_HOME` as the home
  directory rather than `$HOME`. (Some programs might still use `$HOME` for the
  default directory.)
- Does not store recent files. That file is just useless clutter for me,
  especially with kodoku.
