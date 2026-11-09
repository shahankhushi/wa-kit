# wa-kit

> **Agent-native WhatsApp campaign kit: template message library designed to pass Meta Business approval, compliant opt-in flows, and automated conversational commerce sequences.**

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Meta Business API](https://img.shields.io/badge/Meta%20Cloud%20API-Compliant-blue.svg)](https://developers.facebook.com/docs/whatsapp)
[![Architecture: Agent Native](https://img.shields.io/badge/Agent-Native-purple.svg)](#)

---

## Why `wa-kit`?

Most open-source WhatsApp tools are bulk senders, Selenium scripts, and unauthorized webhooks that get business phone numbers banned within 48 hours.

Across conversational-first markets in MENA, Latin America, and South Asia, WhatsApp functions as a primary customer communication and commerce channel. Building for these markets requires strict adherence to Meta's Business Messaging Policies, categorization rules, and user opt-in standards.

`wa-kit` is **not a bulk spam sender**. It is the **architectural, compliance, and design layer** that sits above whichever sender you use (Meta Cloud API, Twilio, Infobip, ManyChat, or custom agents).

---

## What's Included

1. **Meta Pre-Approved Template Schemas (`templates/marketing_templates.json`):**
   - Utility vs Marketing category structures.
   - Dynamic parameters, quick-reply buttons, and URL action triggers.
   - Formatted to pass Meta's automated template approval criteria on initial submission.
2. **Double Opt-In & Compliance Blueprints (`templates/opt_in_flows.md`):**
   - GDPR, TCPA, and Meta Business Policy compliant consent language.
   - Automated unsubscribe and opt-out state management (`STOP`, `UNSUBSCRIBE`).
3. **Conversational Drip Sequences:**
   - Abandoned checkout recovery (with time-decay courtesy coupons).
   - Subscription reorder reminders.
   - Lead qualification and appointment scheduling flows.

---

## Integration with AI Agents

Load `wa-kit` into Claude Code or Cursor to generate compliant WhatsApp marketing campaigns:

```bash
claude "Read wa-kit/templates/marketing_templates.json and adapt the abandoned checkout sequence for our client context"
```

---

## License
MIT © [Imam Haider (@darhaiderimam)](https://github.com/darhaiderimam) • [LinkedIn](https://www.linkedin.com/in/darhaiderimam)
