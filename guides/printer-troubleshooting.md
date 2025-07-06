# Printer Troubleshooting Guide

Help users diagnose and fix common printer issues on Windows by walking through connection checks, queue management, and driver updates.

---

## Prerequisites

- Windows 10 or 11 PC with administrative rights  
- Printer powered on and physically connected (USB or network)  
- Printer driver installed (or access to manufacturer’s website)  

---

## 1. Verify Power & Physical Connections

1. Ensure the printer is **turned on** and the power cable is firmly plugged into both the printer and a working outlet.  

2. Check the data connection:  
   - **USB printers:** Confirm the USB cable is securely seated at both ends.  
   - **Network printers:** Verify the Ethernet cable is plugged into the printer’s LAN port and your network switch or router.  

3. Look for status lights or error codes on the printer’s display panel.  

![Step 1: Check Power & Cables](../assets/screenshots/printer-troubleshooting-step1.png)

---

## 2. Clear the Print Queue

1. Open **Settings → Devices → Printers & scanners**.  

2. Select your printer and click **Open queue**.  

3. In the print queue window, click **Printer → Cancel All Documents**.  

4. Wait 30 seconds for the queue to clear, then close the window.  

![Step 2: Clear Print Queue](../assets/screenshots/printer-troubleshooting-step2.png)

---

## 3. Restart the Print Spooler Service

```powershell
# In an elevated PowerShell window:
Stop-Service -Name Spooler
Start-Service -Name Spooler
```
- Opening elevated PowerShell: right-click the Start button → Windows PowerShell (Admin).
- Restarting the spooler clears hung jobs and resets the printer service.
Step 3: Restart Spooler Service

---

## 4. Update or Reinstall Printer Drivers
1. Go to the printer manufacturer’s support site and download the latest driver for your model.
2. In Settings → Devices → Printers & scanners, select your printer and click Remove device.
3. Run the downloaded driver installer and follow on-screen prompts to reinstall.

Step 4: Reinstall Drivers

---

## 5. Perform a Test Print
- Open Notepad or any text editor.
- Type a line of text and select File → Print.
- Choose your printer and click Print.
- Verify the test page prints correctly.

Step 5: Test Print

---

##Tips & Common Pitfalls
- If the printer is network-connected, verify its IP address in the printer’s menu and ping it from Command Prompt:
ping 192.168.xx.xx
- For USB printers that still won’t print, try a different USB port or cable.
- Ensure Windows Update hasn’t rolled back printer drivers—check Device Manager → Printers for driver status.
- If issues persist, consult the printer’s built-in diagnostics or service logs via its web interface (network models).
