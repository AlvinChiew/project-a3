# Auto Email — User Guide

A simple guide to get your first follow-up email sequence running.

## Install

1. Download the installer from the GitHub Releases (download link is under the video description too!):

- **Auto Email_1.0.0_x64-setup.exe** (recommended)

1. Run the installer and open **Auto Email** from the Start menu.

## First-time setup

### 1. Activate

On first launch the app is **locked** until you activate:

1. Click **Get activation code** — opens the Project A3 page in your browser.
2. Complete the short form (name, business email, company, role, and related fields).
3. Enter your **business email** and `A3-XXXX-XXXX` code (must match the email you used on the Project A3 page).

Activation is free. It links your install to your business profile so A3 can improve the tools for you.

You only enter the code **once**. The app remembers activation in a local database on your device — you will not be asked again on normal restarts.

### Create App Password

1. Enable [2-step verification](https://myaccount.google.com/u/0/signinoptions/twosv)
2. Create [App Password](https://myaccount.google.com/apppasswords)
3. Paste the App Password **WITHOUT** any space

### 2. Configure email (SMTP)

Go to **Settings** and enter your email provider details:

| Field      | Example (Gmail)                          |
| ---------- | ---------------------------------------- |
| SMTP host  | `smtp.gmail.com`                         |
| Port       | `587`                                    |
| Use TLS    | Yes                                      |
| Username   | [your@gmail.com](mailto:your@gmail.com)  |
| Password   | App password (not your regular password) |
| From email | [your@gmail.com](mailto:your@gmail.com)  |

Click **Save settings**, then **Send test** to your own email. You must pass the test before starting a campaign.

### 3. Import contacts

Go to **Lists** → **New list** → open the list → **Import CSV**.

Your CSV should look like:

```csv
email,name
jane@company.com,Jane Smith
bob@company.com,Bob Lee
```

Use Excel and save as CSV for better experience.
You can also add contacts one at a time.

## Create and run a campaign

1. Go to **Campaigns** → **Sample sequence** (or create your own).
2. Open the campaign and review the email steps (Day 0, Day 2, Day 5, etc.). Click **Add step** to add an extra day.
3. Under **Recipient lists**, check the list(s) to send to → **Save lists**.
4. Edit subjects and bodies as needed. Use **Attach file** to add images or PDFs. Click **Save step** after editting each step.
5. Click **Start campaign** on the top right corner.

### Important

- **Keep the app open** while a campaign is running. Emails are sent from your computer on schedule.
- Day offsets are counted from the exact moment you click **Start** (Day 0 sends immediately if due). Each later step is due 24 hours per day offset after that same time — e.g. start at 9pm and Day 1 is due at 9pm the next day, Day 2 at 9pm two days later, and so on.
- **Missed steps are never skipped.** If the app is closed when a step is due, nothing is sent at that time, but the step is _not_ ignored — it is sent (a little late) the next time you open the app. Example: if Day 1 is missed, it is not skipped to Day 2; Day 1 still goes out when you reopen.
- **Catching up:** when you reopen, every step that is now past due is sent back-to-back, spaced by the delay between sends — this includes both any missed step(s) (e.g. an overdue Day 1) and any step that has since come due (e.g. Day 2). So a late Day 1 and an on-time Day 2 can go out together in the same catch-up. Open Auto Email tool around your scheduled time to keep sends on time.
- Use **Cancel** to stop a running campaign.

## Track progress

- On the campaign page, see the progress bar and send logs.
- **Export CSV** downloads a log file with recipient, status, and any errors.

## Common issues

| Problem             | What to try                                                                                       |
| ------------------- | ------------------------------------------------------------------------------------------------- |
| Test email fails    | Double-check app password, port 587, TLS on. Less secure apps must be off — use app passwords.    |
| Emails not sending  | App must stay open. Check campaign status is **running**.                                         |
| Activation required | Click **Get activation code** on the welcome screen and complete the form on the Project A3 page. |
| Gmail blocks sends  | Send smaller batches; increase delay between sends in campaign settings.                          |

## Get help & Update

- **About** → contact links for A3 team
- Use **Click for update** to get the latest version
- Business inquiries: [contact.project.a3@alvinchiew.com](mailto:contact.project.a3@alvinchiew.com)

---

_Created by [Project A3](https://project-a3.alvinchiew.com)_
