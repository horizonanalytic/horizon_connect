# Privacy Policy

**Horizon Connect: Secure Chat**

*Last updated: January 27, 2026*

## Overview

Horizon Connect is built with privacy as its foundation. We believe your conversations are yours alone. This policy explains what data we collect (very little), what we don't collect (almost everything), and how we protect your privacy.

## What We Do NOT Collect

- **Message content**: All messages are end-to-end encrypted using the Signal Protocol. We cannot read your messages. Period.
- **Phone numbers or email addresses**: No account registration required.
- **Contact lists**: We don't access or store your contacts.
- **Location data**: We don't track where you are.
- **Usage analytics**: We don't track how you use the app.
- **Advertising identifiers**: We don't use any advertising or tracking SDKs.
- **Message metadata**: We don't log who talks to whom, when, or how often.

## What We Collect

### Device Identifier
When you install Horizon Connect, a random cryptographic identifier is generated on your device. This identifier:
- Is used solely to route encrypted messages to your device
- Is not linked to any personal information
- Is stored only on your device and our relay server
- Can be reset by reinstalling the app

### Encrypted Message Blobs
Our relay server temporarily stores encrypted messages until they are delivered to the recipient. These messages:
- Are fully end-to-end encrypted before leaving your device
- Cannot be decrypted by us or anyone other than the intended recipient
- Are automatically deleted after delivery or after a maximum retention period (typically 30 days for undelivered messages)

## End-to-End Encryption

Horizon Connect uses the Signal Protocol, the gold standard in secure messaging:
- **Double Ratchet Algorithm**: Provides forward secrecy and future secrecy
- **X3DH Key Agreement**: Secure initial key exchange
- **Curve25519, AES-256, HMAC-SHA256**: Industry-standard cryptographic primitives

Your encryption keys are generated and stored exclusively on your device using the Secure Enclave (when available) or the iOS Keychain.

## Message Retention

By default, messages are ephemeral and disappear after 24 hours. You can configure retention settings per conversation:
- View once (immediate deletion after viewing)
- 5 minutes
- 24 hours (default)
- 7 days
- Persistent (requires mutual consent from both parties)

## Third-Party Services

### Apple Push Notification Service (APNs)
We use APNs to notify you of new messages. Push notifications:
- Contain no message content (only a signal that a new message is available)
- Are required for iOS background message delivery
- Are subject to Apple's privacy policy

### No Other Third Parties
We do not use any analytics services, crash reporting services, advertising networks, or other third-party SDKs that could compromise your privacy.

## Data Storage

### On Your Device
- Encryption keys: Stored in the Secure Enclave or iOS Keychain
- Messages: Stored in an encrypted SQLite database using SQLCipher
- Contacts: Stored locally, never uploaded

### On Our Servers
- Random device identifiers (for message routing)
- Encrypted message blobs (temporarily, until delivered)
- No logs of message metadata, IP addresses, or usage patterns

## Contact Key Exchange

Horizon Connect requires physical proximity to add contacts. When you exchange keys via Bluetooth:
- Public keys are exchanged directly between devices
- No server is involved in the key exchange
- Both parties must confirm the connection
- This ensures you always know who you're talking to

## Your Rights

You have complete control over your data:
- **Delete messages**: Messages can be deleted at any time
- **Delete contacts**: Remove any contact and associated conversation history
- **Delete account**: Uninstall the app to remove all local data; your device identifier will be purged from our servers within 30 days of inactivity

## Children's Privacy

Horizon Connect is not directed at children under 13. We do not knowingly collect information from children under 13.

## Changes to This Policy

We may update this privacy policy from time to time. We will notify you of any material changes through the app or by updating the "Last updated" date.

## Open Source

Horizon Connect's encryption implementation uses open-source, audited libraries. We believe in transparency and welcome security researchers to review our approach.

## Contact Us

If you have questions about this privacy policy or our privacy practices, please contact us at:

**Email**: privacy@horizonanalytic.com

**GitHub**: https://github.com/horizonanalytic/horizon_connect

---

*Horizon Connect is committed to protecting your privacy. We collect the minimum data necessary to deliver messages securely, and we will never sell, share, or monetize your data.*
