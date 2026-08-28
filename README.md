# 🛡️ Raksha – Your Digital Rakhi

**A free, private safety companion for every sister.**  
Gifted with love on Raksha Bandhan.

---

## What is Raksha?

Raksha is a Progressive Web App (PWA) designed as a digital rakhi — a protective tool that any brother can gift to his sister(s).

It works on Android and iPhone, installs on the home screen like a real app, stores everything only on the device, and needs no account or server.

---

## Version History (V1 → V6)

### V1 – The Beginning
**Goal:** Create a useful, free digital rakhi for every sister.

**What was built:**
- Big red SOS button (hold 2 seconds)
- Trusted Circle (add up to 7 contacts)
- Fake incoming call
- Emergency siren + flashlight
- Safety Check-In timer
- Indian helplines (112, 1091, 181, 1098…)
- Private period & wellness tracker
- Everyday safety tips
- Offline support + Add to Home Screen

**Limitation:** SOS only prepared a location share. Not strong enough for real emergencies.

---

### V2 – Custom Voice Trigger
**Goal:** Add a “Hey Siri” style secret phrase.

**What was improved:**
- Custom voice trigger (example: “Bhairava help me”)
- User can set any secret phrase
- Voice Guard ON/OFF
- Suggested phrases included
- Privacy: voice processed only on the device

**Limitation:** Still relied on generic share methods. On iPhone it often opened the system share sheet instead of the exact contacts in Circle.

---

### V3 – Multi-WhatsApp SOS
**Goal:** Send alerts to every person in the Trusted Circle.

**What was improved:**
- Multi-contact WhatsApp flow
- Progress overlay showing each contact
- Message + live location pre-filled
- Clipboard copy of the emergency message
- Clearer emergency buttons (“I’m in Trouble”)

**Limitation:** Still required the user to tap “Send” on every WhatsApp chat. On iPhone the system share sheet remained a problem.

---

### V4 – Better Contact Handling
**Goal:** Fix the iPhone share-sheet problem and target only Circle contacts.

**What was improved:**
- Removed generic system share sheet behaviour
- Direct WhatsApp links (`wa.me` + `whatsapp://`) for each contact
- Individual WhatsApp + SMS buttons for every person in Circle
- Clear panel showing only the user’s chosen contacts
- Stronger guidance: “Tap WhatsApp → then tap Send”

**Limitation:** In a real emergency the sister may not be able to tap multiple times or unlock the phone.

---

### V5 – Instant Primary Contact (Best Free Emergency Approach)
**Goal:** Reduce the number of actions needed in a real emergency.

**What was improved:**
- Introduced **Primary contact** (first person in Circle)
- One hold / one button → instantly opens Primary contact’s WhatsApp
- Message + live location already written
- Only one “Send” tap needed
- “Make Primary” button to change the main contact easily
- Secondary contacts still available if she has time

**Why this mattered:**  
In real danger a person may only manage 1–2 actions. Instant Primary is the fastest reliable free method possible in a web app.

---

### V6 – SOS Alerter Style Flow (Current Version)
**Goal:** Make the experience as close as possible to open-source native apps like SOS Alerter.

**What was improved:**
- **Shake to SOS** (same style as SOS Alerter)
- Voice phrase trigger (already present, refined)
- Hold red button trigger
- Instant Primary WhatsApp opening
- Clear “Alerter Style” emergency card explaining all triggers
- Better visual and vibration feedback
- Updated guidance and README

**Current trigger options:**
1. Shake the phone
2. Say the secret voice phrase
3. Hold the red SOS button

**Still honest limitation:**  
A pure web app cannot send SMS automatically when the phone is locked. For true background automatic SMS, the open-source native app **SOS Alerter** (available on F-Droid) is recommended as a companion.

---

## How to Use Raksha V6

### One-time setup
1. Open the link in **Chrome (Android)** or **Safari (iPhone)**
2. Add to Home Screen
3. Go to **Circle** tab → add the most important person **first** (this becomes Primary)
4. Optionally add more trusted people
5. On Home screen → tap **Enable Shake to SOS** (allow motion permission)
6. Go to **Voice** tab → set your secret phrase (e.g. “Bhairava help me”)

### In an emergency
- Shake the phone, **or**
- Say the voice phrase, **or**
- Hold the red SOS button

→ Primary contact’s WhatsApp opens with the full emergency message + live location already written.  
→ Just tap **Send**.

---

## Features Overview

| Feature | Status |
|---------|--------|
| Instant Primary WhatsApp SOS | ✅ |
| Shake to SOS | ✅ |
| Custom Voice Trigger | ✅ |
| Trusted Circle (up to 7) | ✅ |
| Fake Call | ✅ |
| Siren + Flashlight | ✅ |
| Safety Check-In Timer | ✅ |
| Indian & Global Helplines | ✅ |
| Private Period Tracker | ✅ |
| Offline Support | ✅ |
| Add to Home Screen (Android + iOS) | ✅ |
| Fully Automatic SMS when locked | ❌ (web limitation) |

---

## Privacy Promise

- No account required
- No server
- No tracking
- All data stays only on the device (LocalStorage)
- Voice is processed on-device only

---

## How to Gift

1. Upload the `raksha` folder to [netlify.com/drop](https://app.netlify.com/drop) (or any free static host)
2. Share the permanent link with your sister
3. Tell her:

> Open in Safari (iPhone) or Chrome (Android) → Add to Home Screen.  
> This is my digital rakhi to you. I love you.

---

## Recommended Companion (for maximum protection)

For true automatic SMS even when the phone is locked, also install the free open-source app:

**SOS Alerter** → available on F-Droid  
https://f-droid.org/packages/org.sosalerter.app/

Raksha (easy digital gift) + SOS Alerter (maximum emergency power) is currently the strongest free combination.

---

## Technical Notes

- Pure HTML + CSS + JavaScript
- Progressive Web App (manifest + service worker)
- Works offline after first open
- No backend, no paid services required

---

Made with ❤️ so every sister can feel a little safer, every day.

**Current version: V6**
