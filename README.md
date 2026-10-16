# haplo-call
A simplified, full-screen communication tool (progressive web app) designed for effortless one-touch video calls to single pre-identified contats, aimed at seniors or those needing an accessible, clutter-free interface ("haplo" is Greek for simple).

Download and install haplo-call here: https://haplo-call.base44.app

Please note: Haplo-call was created using vibe coding in base44 for personal use. It was not designed to server other people's needs and it's only made publicly available, in case anyone else finds it useful. The code remains on base44, as I do not have a paid plan. The documentation below is a copy of the documentation I created with base44 and which is included in the admin panel of the app (it was written by AI but I have made minor edits to the version presented here).

## Help & Documentation** 
This guide explains how haplo-call works and how to set it up.

### What haplo-call does
The main screen shows a single large button. Tap it and the app opens the configured call — FaceTime, WhatsApp, a phone call, Google Meet, Zoom, Skype, a custom URL, or an in-app WebRTC video call. Nothing else is shown, so there's nothing to tap by mistake (in theory! - in practice the OS will still allow users to perform gestures that may bring other screens to focus etc).

When a call opens, the app briefly shows a "Calling…" state, then hands off to the chosen calling app or link.

## Configuring the call
Configuration is hidden from the main screen. To open the administrator panel, perform the concealed gesture: tap the top-left corner twice, then tap the bottom-left corner twice. You'll be asked for the administrator PIN (which must be set the first time you open the panel).
In the panel you can set the contact name, the button label, the call method, the destination, an optional deep-link or fallback URL, and the button icon. Use "Test Call" to try the configuration before relying on it.

## The administrator PIN
On first use you must set your own 6-digit PIN — there is no default PIN. The PIN only unlocks the configuration panel; it is light access control, not for sensitive data. You can change it any time from the panel.

## In-app WebRTC calls
Choosing "In-app video (WebRTC)" makes the CALL button start a live video call inside the app and automatically text the join link to the recipient's mobile number. UK numbers entered as 07700 900123 are converted automatically. Twilio credentials are stored securely as app secrets — add or update them in the Secrets dashboard page.

## Installing the app
haplo-call is a Progressive Web App. On a phone, use the browser's "Add to Home Screen" option to install it. Installed, it opens in a clean fullscreen view with no browser chrome.

## Privacy
Your configuration is stored privately in this device's browser only — not on a shared server. Fresh installs start with a blank template. No account or login is required.

## Troubleshooting
If a call doesn't open, check that the destination is correct and that the relevant calling app is installed on the device. For WebRTC, confirm the recipient's mobile number and that Twilio secrets are set. The configuration panel's "Test Call" button helps verify a setup before relying on it.

