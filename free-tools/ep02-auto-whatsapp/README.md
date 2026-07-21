# Auto WhatsApp — User Guide

A simple guide to get your first WhatsApp follow-up sequence running.

## 1. Install

1. Download the Windows installer from the Project A3 release page.
   - Example: **Auto WhatsApp_1.0.0_x64-setup.exe** (recommended)
2. Run the installer and open **Auto WhatsApp** from the Start menu.

## 2. Activate (required)

The app stays locked until you activate — this is free and ties your install to a short profile.

1. Click **Get activation code**.
2. Complete the short form (name, business email, company, role, and related fields).
3. Read the disclaimer (including WhatsApp automation risk), tick **I acknowledge and accept the disclaimer**, then enter your **business email** and `A3-XXXX-XXXX` code (must match the email you used on the Project A3 page).
4. Click **Activate**.

## 3. Link WhatsApp

1. Open **Settings**.
2. Scan the QR code with your phone: WhatsApp → **Linked devices** → **Link a device**.
3. When you see **Connected**, optionally send a **test message** to your own number (include country code, e.g. `60123456789`).
4. You must be connected before starting any campaign.

**Important:** Keep Auto WhatsApp open while campaigns run. Messages are only sent while the app is running on this computer.

## 4. Add a contact list

1. Go to **Lists** → create a list.
2. Import a CSV or add numbers manually.

CSV format:

```csv
phone,name
15551234567,Jane
15559876543,John
```

- Column 1 = phone (required) — digits with country code
- Column 2 = name (optional)
- Header row is optional

## 5. Create a campaign

1. Go to **Campaigns** → **New campaign** (or use **Create sample** for a starter sequence).
2. Open the campaign and edit message steps (Day 0, Day 2, Day 5, …). Add media if needed.
3. Attach one or more contact lists.
4. Set a delay between sends (default **10 seconds** is safer for WhatsApp than very short gaps).
5. Click **Start**.

## 6. Track progress

- Open a running campaign to see progress and send logs.
- Export logs to CSV anytime (**Export CSV**). The file footer includes Auto WhatsApp · A3 branding.

## Catch-up behavior

- **Catching up:** when you reopen the app, every step that is now past due is sent back-to-back, spaced by the delay between sends. Open Auto WhatsApp around your scheduled times to keep sends on time.

## Troubleshooting

| Problem                     | What to try                                                              |
| --------------------------- | ------------------------------------------------------------------------ |
| QR never appears            | Confirm the WhatsApp bridge started (restart the app).                   |
| Scan works then disconnects | Keep your phone online; re-scan from Settings → Disconnect → new QR.     |
| Test message fails          | Use full country code digits; recipient must be a valid WhatsApp number. |
| Campaign won't start        | Link WhatsApp in Settings; add at least one step and one list.           |
| Messages not sending        | Keep the app open; check send logs for errors; increase send delay.      |
| Account warnings            | Lower volume, increase delay, message only consented contacts.           |

## Updates

Use **Click for update** in About (or the update control in the app) to check for a newer installer and download it in your browser.

## Disclaimer (summary)

Auto WhatsApp is free and provided “as is.” You accept all risk, including possible account restrictions. Full text is shown at activation and in About.
