# Joomla! Plugin: Media Action - Resizefix

A Joomla 4 plugin that serves as a **bugfix override** for the core `plg_media-action_resize` plugin. This plugin resolves a bug present in the Joomla 4 core image resize action which has been officially fixed in Joomla 5.3, but is not patched in Joomla 4 due to its security-only maintenance policy. See this [pull request](https://github.com/joomla/joomla-cms/pull/45311) for details about the fix.

---

## Plugin Name

**`plg_media-action_resizefix`**

- Plugin Group: `media-action`
- Folder Path: `plugins/media-action/resizefix/`
- Joomla Version: **4.x compatible**
- Status: Drop-in replacement (does not modify core files if installed correctly)

---

## Features

- Backports the Joomla 5.3 fix for media image resizing.
- Fully standalone — avoids overwriting Joomla core plugins if installed properly.
- Uses PSR-4 autoloading (`Joomla\Plugin\MediaAction\Resizefix`).

---

## Installation

1. Download the latest release ZIP.
2. Go to your Joomla Admin Panel → **Extensions → Install**.
3. Upload and install `plg_media-action_resizefix.zip`.
4. **Enable the plugin** under **System → Plugins** - search for "media action" and enable the plugin named **Media Action - Resize (J4 Bug Fix)**.
5. (Optional but recommended) **Disable the core `plg_media-action_resize`** to avoid conflicts.
