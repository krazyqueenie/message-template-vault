# Message Vault

Message Vault is a lightweight, local-first alternative to sticky notes and scattered drafts. 
It’s a single HTML file that lets you store, search, and copy/paste **formatted** templates and reference content (bold, underline, lists, tables, links, etc.).

No installs. No accounts. No servers. Just open the file in a browser and use it.

---

## What it’s for

- Message templates you reuse all the time
- CRM/portal replies that need formatting
- Reference lists (phone numbers, resort contacts, policies)
- Tables that you want to keep as tables (not flattened into plain text)

---

## How it stores your data

Message Vault saves your templates in two ways:

1. **Local browser storage (localStorage)**  
   - Your templates persist through refresh/closing the tab.
   - Stored only in your browser on that device.
   - Clearing browser data or cache will delete data, use JSON as backup. 

2. **JSON Export/Import**  
   - Export creates a backup file you can keep anywhere.
   - Import restores or transfers your vault to another computer/browser.

✅ Best practice: **Export regularly** so you always have a backup.

---

## Getting started

1. Download `message-vault.html`
2. Open it in a browser (Chrome/Edge recommended)
3. Click **New** to create your first template
4. Add a title, optional tags, and your formatted message
5. Click **Save**
6. Original JSON file will autocreate on 1st save

---

## Basic use

### Create a template
- Click **New**
- Give it a **Title**
- Add **Tags** (comma separated) if you want
- Type/paste your message (formatting is preserved)
- Click **Save**

### Edit a template
- Click a template from the left list
- Make changes (title/tags/body)
- Click **Save**

> Important: changes are not permanent until you click **Save** (or **Save Version**).

### Copy for pasting
- Click **Copy**
- Paste into your CRM / portal / email

(Message Vault attempts to copy rich text + plain text + emojis. Some systems only accept plain text.)

---

## Version History (snapshots)

If you want to keep a “checkpoint” copy of a template:
- Click **Save Version**

This stores a snapshot in the **Version History** panel where you can:
- **Restore** a version into the editor
- **Copy** a version
- **Delete** a version

> Note: Restore loads the snapshot into the editor — click **Save** if you want to make the restore permanent.

---

## Search

Use the search bar to find templates by:
- title
- tags
- text inside the template body

---

## Export / Import (recommended)

### Export (backup)
- Click **Export**
- A file downloads: `message_vault_export.json`

Keep this file somewhere safe (Drive, folder, USB, etc.).

### Import (restore / move to a new device)
- Click **Import**
- Select your saved JSON file
- Your vault loads immediately and is saved to local storage

✅ Recommendation for first-time setup:  
If you’re moving to a new computer or browser, **Import your JSON first** so your vault is loaded before you start adding new templates.

---

## Safety tips (so you don’t lose work)

- **Click Save** after edits. If you close/refresh before saving, those unsaved changes may be lost.
- Export your JSON periodically as a backup (especially before big edits).
- If you use multiple computers/browsers, export/import is how you sync.

---

## FAQ

### Does it work offline?
Yes. It’s just a local HTML file.

### Does it save if I refresh or close the tab?
Yes — anything you have clicked **Save / Save Version / New / Duplicate / Delete / Import** on is stored in localStorage and will survive refresh.

Unsaved typing that you didn’t click **Save** on may not.

### Can I use emojis?
Yes. It stores HTML content, so formatting, tables, and many CRM-safe emoji/image methods are preserved.

### Where is my data stored?
In your browser’s local storage under the key:
`message_vault_v1`

Export/Import lets you move it anywhere as a JSON file.

---

## License
Use it, modify it, share it. DO NOT sell it, this was created originally by KrazyQueenie and provided as a FREE tool.
