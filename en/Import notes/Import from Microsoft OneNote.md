---
permalink: import/onenote
---

Obsidian allows you to easily migrate your notes from Microsoft OneNote by importing them directly from your Microsoft Account.

## Import your OneNote data into Obsidian

You will need the official Obsidian [[Importer]] plugin, which you can [install here](obsidian://show-plugin?id=obsidian-importer).

1. Open **Settings**.
2. Go to **Community Plugins** and [install Importer](obsidian://show-plugin?id=obsidian-importer).
3. Enable the Importer plugin.
4. Open the **Importer** plugin using the command palette or ribbon icon.
5. Under **File format** choose **OneNote.**
6. Click **Sign in** to open your web browser to the Microsoft sign-in page. Enter the credentials for your Microsoft account which contains your OneNote Notebooks. More information about the Microsoft sign-in process is available below.
7. Click **Accept** to grant Obsidian permission to view your OneNote Notebooks.
8. Click **Open Link** to allow your browser to redirect you to the Obsidian app.

    ![[OneNote-Importer-Open-Link.png]]

9. In the Obsidian app, the Importer dialog will now display that you are signed in and list your OneNote Notebooks and Sections. Check the sections you wish to import.

    ![[OneNote-Importer-Select-Sections.png]]

10. Click **Import** and wait until import is complete.
11. You're done!

## Export your data from OneNote

Microsoft offers limited options to export OneNote files. We are currently working on OneNote support via the [[Importer|Importer plugin]].

In the meantime, you can [Convert OneNote to Markdown](https://github.com/theohbrothers/ConvertOneNote2MarkDown) using a PowerShell script.

## Import your OneNote data into Obsidian

You will need the official Obsidian [[Importer]] plugin, which you can [install here](obsidian://show-plugin?id=obsidian-importer).

Depending on the tool you used, the export may be in Markdown format or HTML format. Follow the instructions below based on the file format you exported to: 

- [[Import HTML files]]
- [[Import Markdown files]]

## Microsoft Account Authentication

The Obsidian Importer plugin uses [OAuth](https://learn.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow) to authenticate with your Microsoft account and import your OneNote notebooks. This grants a short term access token to your account which is used only from your computer and is never stored. After the import completes you may optionally revoke the token from the [Microsoft apps & services page](https://account.live.com/consent/Manage). 
