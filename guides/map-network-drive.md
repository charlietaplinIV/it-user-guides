# Map a Network Drive

This guide walks end users through mapping a shared network folder as a drive in Windows, providing quick access to files on a server or another PC

---

## Prerequisites

- Windows 10 or 11 PC
- Network share path (e.g., \\ServerName\ShareName)
- Valid credentials (domain or local account) with access to the share


---

## 1. Open File Explorer

- Click the folder icon on the taskbar or press Win + E.-
-  Select This PC in the left pane.

Step 1: Open File Explorer

---

## 2.  Launch Map Network Drive Wizard

- On the This PC toolbar, click Map network drive.
- In the dropdown, choose Map network drive….
  
Step 2: Map Network Drive button


---

## 3. Configure Drive Letter and Folde

- In the wizard dialog:
- Drive: Choose an available letter (e.g., Z:).
- Folder: Enter the share path, e.g.,
\\ServerName\ShareName
- (Optional) Check Reconnect at sign-in to remap automatically on login.
- (Optional) Check Connect using different credentials if your Windows login differs.
- Click Finish.
  
Step 3: Enter Drive Letter and Folder


---

## 4. Verify the Mapped Drive

- In This PC, you should now see the new drive under Network locations with the chosen letter.
- Double-click to open and confirm you can read/write files.

Step 5: Mapped Drive Visible

 

---


## Tips & Troubleshooting

- If you receive “Access Denied”, double-check your username format and that the share permissions grant your account access.
- For intermittent disconnects, ensure Reconnect at sign-in is enabled and that the network is stable.
- If the drive letter is already in use, pick a different letter or disconnect the existing mapping via This PC → Map network drive → Disconnect network drive.
- On a domain-joined PC, omitting the domain prefix may lead to authentication failures—always use DOMAIN\Username.

Once you’ve confirmed the drive maps successfully, you can proceed to personalize a folder shortcut or pin the drive to Quick access for faster navigation.


