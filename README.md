# Nextcloud CSS Redesign

One Custom CSS stylesheet for Nextcloud Hub. It adds pill buttons, card surfaces, one radius scale across every app, and light and dark mode that follow your device.

> **Not maintained.** This project is shared as is and won't be updated. Issues and pull requests won't be answered. Fork it if you want to change it.

> **Not affiliated with** or endorsed by Nextcloud GmbH. Nextcloud is a trademark of Nextcloud GmbH.

<img width="2400" height="3720" alt="image" src="https://github.com/user-attachments/assets/694cc9d5-8039-4abb-a20d-3f680acffc73" />

## Install

1. **Get the Custom CSS app** (you must be an admin):
   - In the web interface: avatar → **Apps** → search **Custom CSS** → **Download and enable**.
   - Or from the command line: `sudo -u www-data php occ app:install theming_customcss`
   - On Nextcloud AIO: `sudo docker exec --user www-data -it nextcloud-aio-nextcloud php occ app:install theming_customcss`
2. **Set the theming colors** in **Administration settings → Theming**:
   - Primary color: `#0071E3`
   - Background color: `#000000`
   - Turn on **Remove background image**
3. **Add the theme:** paste all of `nextcloud-theme-v2.min.css` into the **Custom CSS** box at the bottom of the Theming page, replacing anything already there. Save, then hard refresh (Cmd+Shift+R on macOS, Ctrl+Shift+R on Windows and Linux).

To remove the theme, clear the Custom CSS box and save.

## Notes

- Built and tested on Nextcloud 35 (Hub 26), AIO install.
- Light and dark mode follow your device's appearance setting, not Nextcloud's own.
- The Collabora document editor can't be restyled, because it loads from its own server.
- Nextcloud and app updates can rename things and break rules over time. Since the project isn't maintained, you'll need to fix those yourself.
