# AI Customer Profiling — User Guide

A simple guide to tag inbound WhatsApp customers with AI — without automatic replies.

## 1. Install

1. Download the Windows installer from the Project A3 release page.

- Example: **ep04-ai-customer-profiling_x64-setup.exe** (**recommended**)

2. Run the installer and open **AI Customer Profiling** from the Start menu.

## 2. Activate (required)

The app stays locked until you activate — this is free and ties your install to a short profile.

1. Click **Get activation code**.
2. Complete the short form (name, business email, company, role, and related fields).
3. Read the disclaimer (including unofficial WhatsApp risk and AI profiling inaccuracy), tick **I acknowledge and accept the disclaimer**, then enter your **business email** and `A3-XXXX-XXXX` code (must match the email you used on the Project A3 page).
4. Click **Activate**.

## 3. Define tags

1. Open **Tags**.
2. Create single-select tags your business cares about — for example:
   - **language** — Preferred language based on how they write — options `English`, `Malay`, `Chinese`, `Mixed`
   - **age** — Approximate age group if stated or clearly implied — options `under-18`, `18-24`, `25-34`, `35-44`, `45-54`, `55+`
   - **stage** — Where they are in the buying journey — options `New lead`, `Comparing`, `Ready to buy`, `Existing customer`
   - **urgency** — How soon they need a response or decision — options `Today`, `This week`, `No rush`
   - **intent** — Main reason they messaged — options `Buy`, `Sell`, `Support`, `Inquire`
3. Put mapping hints in the description (e.g. “55+ means 55 or older”) so phrases like “I’m 60” can map correctly.

## 4. Link WhatsApp

1. Open **Settings**.
2. Under **WhatsApp connection**, scan the QR code with your phone: WhatsApp → **Linked devices** → **Link a device**.
3. When you see **Connected**, optionally send a **test message** to your own number (include country code, e.g. `15551234567`).

**Important:** Keep AI Customer Profiling open while you want chats stored and profiled. This app never sends automatic replies to customers.

## 5. Add your OpenAI API key (BYOK)

AI Customer Profiling uses **your** OpenAI account — bring your own key (BYOK). The key is stored in the OS keychain, not in plain files.

1. Open **Settings** → **OpenAI (BYOK)**.
2. Paste your API key (starts with `sk-…`).
3. Leave the model as **gpt-4o-mini** unless you prefer another Chat Completions model.
4. Click **Save**, then **Test** until you see the connection OK.

Get a key from your OpenAI account dashboard. You pay OpenAI directly for usage.

## 6. Turn profiling on

1. Open **Conversations**.
2. Turn **Profiling on**.
3. When customers message you in 1:1 chats, conversations appear in the list.
4. After a short quiet window, tags update. Open a chat for history, tag chips, and **Re-profile**.

Each profile run sends **all enabled tags** plus the recent chat transcript (up to 40 message bubbles) in **one** OpenAI request (it does not wait for a fixed number of messages, and it does not call OpenAI once per tag).

Tips: hedging (“maybe this week or next month”) leaves a tag empty; the latest clear statement wins over older ones.

## Troubleshooting

| Problem                      | What to try                                                                                     |
| ---------------------------- | ----------------------------------------------------------------------------------------------- |
| QR never appears             | Restart the app.                                                                                |
| Scan works then disconnects  | Keep your phone online; Settings → Disconnect → scan a new QR.                                  |
| OpenAI Test fails            | Check the key, billing on your OpenAI account, and model name.                                  |
| No chats / empty tags        | Confirm WhatsApp **Connected**, Profiling on, key tested, tags defined, and the app stays open. |
| Wrong tag after a correction | Wait for the quiet window or click **Re-profile**.                                              |
| Account warnings             | Lower volume; use only for chats you already handle; review WhatsApp’s terms.                   |

## Updates

Use **Click for update** in About (or the update control in the app) to check for a newer installer and download it in your browser.

## Disclaimer (summary)

AI Customer Profiling is free and provided “as is.” You accept all risk, including possible account restrictions and inaccurate AI tags. Full text is shown at activation and in About.
