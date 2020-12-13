# Dotfiles

This repository houses my own personal dotfiles. The dotfiles are managed
utilizing [dotbot](https://github.com/anishathalye/dotbot). See that link
for more detailed instructions.

## Get Started

Clone: `git clone https://github.com/ocelotslot/dotfiles.git`

Install Dependencies:
- mlocate
- zsh
- zsh-completions
- python-i3-py (aur)
- xautolock
- rofi
- dunst
- scrot
- imagemagick
- python
- i3-gaps (or just i3, you'll need to make some adjustments)
- i3bar
- i3lock
- ttf-font-awesome
- urxvt
- urxvt-perls

Create Symlinks: `./install`

### mlocate

For systems using systemd-homed LUKS containers it makes sense to
restrict the database so that it cannot scan the contents of the LUKS
container. This would leak information about what files are present
when that user is not logged in.

Edit `/etc/updatedb.conf` and add `/home` to the list of excluded
directories.

Dotbot will handle creation of a user-local systemd-timer to create
a user-local mlocate database that resides inside of the LUKS
container.

Dotfiles Template
=================

[dotbot]: https://github.com/anishathalye/dotbot
[fork]: https://github.com/anishathalye/dotfiles_template/fork
[anishathalye_dotfiles]: https://github.com/anishathalye/dotfiles
[csivanich_dotfiles]: https://github.com/csivanich/dotfiles
[m45t3r_dotfiles]: https://github.com/m45t3r/dotfiles
[alexwh_dotfiles]: https://github.com/alexwh/dotfiles
[azd325_dotfiles]: https://github.com/Azd325/dotfiles
[bluekeys_dotfiles]: https://github.com/bluekeys/.dotfiles
[wazery_dotfiles]: https://github.com/wazery/dotfiles
[thirtythreeforty_dotfiles]: https://github.com/thirtythreeforty/dotfiles
[dotbot-users]: https://github.com/anishathalye/dotbot/wiki/List-of-Dotbot-Users
