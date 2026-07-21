# AI WhatsApp — User Guide

A simple guide to get AI auto-replies working on your WhatsApp DMs.

## 1. Install

1. Download the Windows installer from the Project A3 release page.

- Example: **ep03-ai-whatsapp_x64-setup.exe** (**recommended**)

2. Run the installer and open **AI WhatsApp** from the Start menu.

## 2. Activate (required)

The app stays locked until you activate — this is free and ties your install to a short profile.

1. Click **Get activation code**.
2. Complete the short form (name, business email, company, role, and related fields).
3. Read the disclaimer (including WhatsApp automation risk and AI reply risk), tick **I acknowledge and accept the disclaimer**, then enter your **business email** and `A3-XXXX-XXXX` code (must match the email you used on the Project A3 page).
4. Click **Activate**.

## 3. Link WhatsApp

1. Open **Settings**.
2. Under **WhatsApp connection**, scan the QR code with your phone: WhatsApp → **Linked devices** → **Link a device**.
3. When you see **Connected**, optionally send a **test message** to your own number (include country code, e.g. `15551234567`).
4. You must be connected before the bot can receive or send replies.

**Important:** Keep AI WhatsApp open while you want replies. The bot only runs while the app is open on this computer.

## 4. Add your OpenAI API key (BYOK)

AI WhatsApp uses **your** OpenAI account — bring your own key (BYOK). The key is stored in the OS keychain, not in plain files.

1. Open **Settings** → **OpenAI (BYOK)**.
2. Paste your API key (starts with `sk-…`).
3. Leave the model as **gpt-4o-mini** unless you prefer another Chat Completions model.
4. Click **Save**, then **Test** until you see the connection OK.

Get a key from your OpenAI account dashboard. You pay OpenAI directly for usage.

## 5. Write your prompts (three sections)

1. Open **Prompts** (home screen).
2. Fill in the three sections:

| Section                          | What to write                                                                        |
| -------------------------------- | ------------------------------------------------------------------------------------ |
| **Rules** — _You must_ / _Never_ | Hard rules the bot must always follow or never do (e.g. never invent prices).        |
| **Communication style**          | Tone and voice (e.g. short, friendly, professional).                                 |
| **Scenario**                     | Who the bot is and what situation it handles (e.g. shop FAQs during business hours). |

1. Click **Save**.
2. Turn **Bot on** (toggle at the top). The bot stays off until you enable it.

Tips: start simple; use Help & Resources in the app for example wording. The bot replies to **all 1:1 chats** (not group chats).

## 6. Leave the app open

- With WhatsApp linked, OpenAI key saved, prompts filled, and **Bot on**, inbound DMs are answered automatically.
- Check **Activity** for recent replies (sent, failed, or skipped). Export to CSV anytime if you need a log.
- Closing the app pauses auto-replies until you open it again.

## Troubleshooting

| Problem                     | What to try                                                                                            |
| --------------------------- | ------------------------------------------------------------------------------------------------------ |
| QR never appears            | Restart the app.                                                                                       |
| Scan works then disconnects | Keep your phone online; Settings → Disconnect → scan a new QR.                                         |
| OpenAI Test fails           | Check the key, billing on your OpenAI account, and model name.                                         |
| Bot on but no replies       | Confirm WhatsApp **Connected**, key tested, prompts saved, and the app stays open. Groups are skipped. |
| Replies look wrong          | Edit Rules / Style / Scenario on **Prompts**, save, and try again.                                     |
| Account warnings            | Lower volume; reply only where you have permission; review WhatsApp’s terms.                           |

## Updates

Use **Click for update** in About (or the update control in the app) to check for a newer installer and download it in your browser.

## Disclaimer (summary)

AI WhatsApp is free and provided “as is.” You accept all risk, including possible account restrictions and incorrect AI replies. Full text is shown at activation and in About.
