# Quick Paste History Privacy Policy

**Last Updated: May 8, 2026**

---

## 1. Information Collection and Use

Quick Paste History is a clipboard management tool whose core function is to record, manage, and retrieve clipboard content locally on your device.

### 1.1 Information We Do **Not** Collect

- Personal identification information (name, ID number, address, etc.)
- Sensitive information such as account passwords, bank card numbers, etc.
- Device identifiers (IDFV, IDFA, etc.)
- Browsing history, location information
- Contacts, photo album, microphone, camera data
- Usage behavior statistics or analytics data

### 1.2 Information We **Access**

Quick Paste History only accesses the following information locally on your device as necessary for its core functionality:

| Data Type | Purpose | Uploaded to Server |
|-----------|---------|:-----------------:|
| **Clipboard Content** | Records text/links copied by the user, supporting search, favorites, and quick fill | Local storage only |
| **iCloud** | Syncs history across your devices via NSUbiquitousKeyValueStore | iCloud private sync only |
| **App Store In-App Purchase** | Verifies Pro feature purchase status (receipt verification only) | No purchase details collected |

> All clipboard data processing is done locally on the device and **will not be uploaded to any external server**.

---

## 2. Data Storage

### 2.1 Local Storage

- Clipboard history records are stored in a SwiftData database within the App sandbox
- The database is not encrypted (Apple sandbox mechanism provides system-level isolation)
- Users can manually clear all history records

### 2.2 iCloud Sync (Optional Feature)

- When enabled, history records are synced across your own iCloud account via `NSUbiquitousKeyValueStore`
- Data is protected by iCloud security mechanisms and cannot be accessed by the developer
- Sync can be turned off at any time in settings
- Turning off sync will not delete local data

### 2.3 Data Retention

- History records are retained by default; users can manually delete individual entries or clear all
- Deletion takes effect immediately and is irreversible

---

## 3. Data Sharing

Quick Paste History **will not share user data with any third party**, including but not limited to:

- Will not sell user data
- Will not use data for advertising or user profiling
- Will not send any clipboard content to third-party APIs
- Will not embed third-party analytics SDKs

---

## 4. Keyboard Extension and Permissions

Quick Paste History provides a Keyboard Extension for quickly pasting history content in any app:

- **Access**: The keyboard extension only runs when activated and only reads clipboard content
- **Network**: The keyboard extension has no network access permissions
- **Data Isolation**: The keyboard extension shares sandbox data with the main App but does not expose it externally

---

## 5. Clipboard Reading

Quick Paste History reads the clipboard at the following times:
- When the app is running in the foreground, it detects clipboard changes and records new content
- When the user actively shares content to Quick Paste History

As required by iOS, the first clipboard read will trigger a system-level permission prompt. Users can manage this permission at any time in System Settings.

---

## 6. Children's Privacy

Quick Paste History does not collect personal information from children.

---

## 7. Privacy Policy Changes

If the privacy policy changes, we will update the "Last Updated" date at the top of the page and notify users through in-app announcements or version update notes.

---

## 8. Contact Us

If you have any questions about the privacy policy, please contact us through the following channels:

- **Developer**: 陈修
- **Email**: chensingyou@126.com
- **App**: Quick Paste History (Developer: Singyou)

---

> **Summary: Your data belongs to you.** Quick Paste History does not upload any content to servers, does not track user behavior, and does not embed third-party SDKs. All clipboard data is processed only on the local device and within iCloud private space.
