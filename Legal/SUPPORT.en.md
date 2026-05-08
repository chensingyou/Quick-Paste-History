# Quick Paste History – Technical Support

---

## 📧 Contact the Developer

- **Email**: chensingyou@126.com

When sending an email, please include:
1. Your iOS version number
2. Your device model
3. A detailed description or screenshot of the issue
4. Steps to reproduce (if applicable)

---

## ❓ Frequently Asked Questions

### 1. Clipboard not recording automatically?

This is a permission restriction in iOS. Please make sure:
1. Quick Paste History has been brought to the foreground at least once
2. You tapped "Allow Paste" on the first launch (system permission prompt)
3. If you previously denied it, go to **System Settings → Quick Paste History → Paste from Other Apps** → change to **Allow**
4. Clipboard history is updated only when the app is in the foreground. You need to open the app interface or its keyboard extension each time you paste.

---

### 2. How to use the keyboard extension?

1. Go to **System Settings → General → Keyboard → Keyboards → Add New Keyboard**
2. Select **Quick Paste History**
3. Tap the Quick Paste History keyboard name → **Allow Full Access**
4. In any text input field, long-press the keyboard switcher and slide up, then switch to the Quick Paste History keyboard to browse and paste historical content

---

### 3. iCloud sync not working?

1. Make sure all your devices are signed into the same Apple ID
2. Make sure iCloud is enabled (System Settings → Profile → iCloud → status should show "Signed In")
3. Open Quick Paste History on different devices and wait about 30 seconds — data will sync automatically
4. If sync hasn't happened after a long time, try restarting the app

> Sync is based on `NSUbiquitousKeyValueStore`. Apple does not provide a manual refresh API, and sync usually completes within tens of seconds.

---

### 4. How to clear all history?

On the main page of the app, tap the settings icon in the top-right corner → in the settings menu, select "Clear All Records". This action cannot be undone.

---

### 5. How to purchase and use Pro features?

1. Tap the settings icon in the top-right corner of the main screen → **Pro Upgrade**
2. Select the Pro version and complete the in-app purchase
3. Features are automatically unlocked after purchase
4. Devices under the same Apple ID can restore purchases (tap "Restore Purchase" on the purchase page)

---

### 6. What is Quick Fill?

Quick Paste History allows you to add frequently used information to Quick Fill in advance, providing a quick-fill entry in the keyboard extension so you can quickly paste commonly used content.

---

### 7. How to use the search feature?

There is a search bar at the top of the main page. Enter keywords to search through text content in your history. Results are sorted by relevance.

---

### 8. Is my data secure?

- All clipboard data is stored only on your device locally and in your iCloud private space
- The developer cannot access your clipboard content
- There is no backend server receiving your data
- Please refer to the Privacy Policy for details

---

## 🐛 Report a Bug

If you find a bug, please send an email to chensingyou@126.com with **[Bug]** in the subject line.

Please include in your email:
- iOS version
- Device model
- Steps to reproduce (the more detailed, the better)
- Screenshots or screen recordings (if available)

---

## 💡 Feature Suggestions

Have new ideas? Feel free to email me for discussion, with **[Suggestion]** in the subject line. I will read every piece of feedback carefully.
