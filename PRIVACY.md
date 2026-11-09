# Faber Companion privacy policy

Effective: November 9, 2026
Developer: Yashwanth Reddy Katipally
Contact: yashwantreddykatipally@gmail.com

Faber Companion is an iPhone app that shows and steers the coding agents running on your own Mac, through Faber for Mac. This policy covers the iPhone app.

## The short version

- No account, no advertising and no tracking.
- Optional usage analytics, off by default on iPhone. If you say yes, the app sends counts and fixed labels about which features you use to the developer's own server. Never your chats, code, files or terminals.
- We cannot see your chats, code, files or terminals. They never go to our server.
- Chats, terminals and approvals between your iPhone and your Mac are end-to-end encrypted.
- Alerts are a short summary of what the agent needs, delivered by Apple through your own private iCloud.

## What the app handles, and where it goes

- Your work (chat messages, approvals, answers, terminal text, file changes, photos you pick, dictated text): sent only to your own Mac, encrypted so that only your iPhone and your Mac can read it. Some of it is cached on your iPhone so screens open quickly. Deleting the app removes the cache.
- Pairing keys: a key pair that identifies your iPhone, and your Mac's public key, are stored in the iPhone Keychain on this device.
- Your iCloud: to find your Mac and open a direct link, the app and Faber for Mac exchange small records in your own private iCloud (CloudKit) database. They hold device names and public keys, short-lived connection offers, and your iPhone's notification token. Fields that describe your work are encrypted. Alerts are saved there too, as a short summary of what the agent needs (for example "Run npm test?") with secret patterns masked and the length capped, so Apple can show them on your iPhone. They expire after a short time and are deleted when you answer. This database belongs to you and is stored by Apple. We have no access to it.
- Direct connection from anywhere: to find a network path, the iPhone and the Mac each ask public STUN servers run by Google and Cloudflare for their public IP address. Those servers see your IP address and nothing else.
- Notifications and Live Activities (optional): by default your Mac saves each alert in your own private iCloud database and Apple delivers it to your iPhone. If you add your own key to Faber for Mac, your Mac sends alerts through the Apple Push Notification service instead, using a push token your iPhone gives Apple. Either way we do not send, receive or store alerts, and an alert is a short redacted summary of what the agent needs. Your Allow, Deny or Reply answer goes back over the direct encrypted link or as an encrypted record in your iCloud. Live Activity updates carry progress status, such as how many agents are running or waiting. They never include your messages, code, file contents or terminal output. Apple handles delivery under its own privacy policy.
- Camera (optional): to scan a pairing code or take a picture to send to your agent. Photos you choose come from the system photo picker, and only the ones you pick are used.
- Microphone (optional): to dictate a message. Speech becomes text on your iPhone using Apple's on-device speech feature. Audio is not recorded, stored or sent.
- Local Network: to find your Mac on your Wi-Fi.

## Optional usage analytics

Faber Companion can send anonymous usage analytics so the developer knows which screens and features get used. It is off until you turn it on.

- Off by default. The app asks once, after you pair a Mac or try the demo. Anything other than Share counts as no. Change it any time in Settings, Privacy.
- Where it goes: the developer's own self-hosted OpenPanel server at https://telemetry.openlive.dev. It is not sold, not used for ads, and not shared with other companies. It does not track you across other companies' apps or websites, and the app does not use App Tracking Transparency.
- What is sent: fixed event names with short fixed labels. An app opened (first time, and once per day of use), a screen was opened, a pairing attempt ended (route and outcome), the notification permission answer, the Live Activity switch changed, an approval was answered (allow, deny or always, and where from), a chat message was sent (never its text), a connection to your Mac failed (a short error code), a setting changed (which one, never its value), an agent turn finished or failed, an agent or tool was used (its name), a preview was opened, a pane was split, a Settings pane was opened, and one last event when you turn sharing off. Every event also carries the app, its version, system version, device type, language and days since first open. Settings, Privacy, What's sent lists all of it.
- What is never sent: prompts and replies, code and file contents, file paths and file names, project, folder and branch names, messages, error text, your name or email, and your IP address or location.
- Your ID: an anonymous ID links the events from your devices. It is a one way SHA-256 hash of your iCloud user record ID, so your iPhone and your Mac show up as one profile without a login. If iCloud is unavailable, a random ID is used instead. We do not use your name, email, advertising identifier (IDFA), vendor identifier (IDFV) or any hardware identifier.
- No location: the app sends the placeholder address 127.0.0.1 and the server drops client IP headers, so no IP address and no place is stored.
- Turn it off: the events waiting on your iPhone and the ID are deleted at once. If you are online, one last event says sharing was turned off. Settings, Privacy also has Reset ID, which starts a new anonymous ID.
- Retention: events are kept on the server for 24 months, then deleted. Server backups keep the newest 14 daily copies on the server and weekly encrypted copies off the machine for 8 weeks, so a deleted event can remain in a backup for up to 8 weeks.
- Deletion: copy your Analytics ID from Settings > Privacy and email it to yashwantreddykatipally@gmail.com. We will delete the data filed under that ID.

## Demo mode

The built-in demo uses sample data inside the app. It does not contact your Mac or your iCloud. It sends nothing to any server except the usage analytics above, if you chose to share.

## What we do not do

We do not sell your data, we do not build advertising profiles, we do not use advertising identifiers, and we do not track you across other companies' apps or websites.

## Your choices and deletion

- Unpair a Mac in Settings, then remove the iPhone in Faber on your Mac.
- Turn off notifications or the Live Activity in iOS Settings or in the app.
- Turn usage analytics off in Settings, Privacy, and ask for deletion of what was sent (see above).
- To delete the records in your iCloud, remove the iPhone in Faber on your Mac, or manage iCloud data in iOS Settings. Deleting the app removes keys and cache from the iPhone.

## Children

The app is not directed to children. Usage analytics are off by default and carry no name, email or contact details.

## Faber for Mac

Faber for Mac is a separate app with its own settings. It sends the same kind of usage analytics to the same server, on the same terms as above, with two differences: it is on by default, and the first-run setup tells you so and lets you turn it off. Turn it off in Settings, Privacy, where What's sent and Reset ID are too. It also offers crash reports. Those are separate: after a crash, Faber shows you the redacted report first and sends nothing unless you press Send.

## Changes

If this policy changes, the date above changes and the release notes say what changed.

## Contact

Questions about privacy: yashwantreddykatipally@gmail.com
