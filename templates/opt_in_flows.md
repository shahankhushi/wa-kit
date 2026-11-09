# WhatsApp Opt-In & Compliance Architecture

Meta strictly enforces opt-in policies for WhatsApp Business API accounts. Sending unsolicited marketing messages results in immediate phone number quality degradation (Red Status) and tier downgrades (from 10k messages/day to 1k/day).

---

## 1. Non-Negotiable Meta Policy Rules

1. **Explicit Consent:** You must obtain explicit opt-in clearly stating the user agrees to receive messages over WhatsApp from your specific business.
2. **Third-Party Consent Forbidden:** You cannot buy phone lists or transfer opt-in from email without explicit WhatsApp confirmation.
3. **Opt-Out Mechanism:** Every promotional broadcast must include a clear opt-out footer (`Reply STOP to opt out`).

---

## 2. Recommended Double Opt-In Flow (Conversational)

```
[Customer checks box on Shopify Checkout / Lead Form]
                  |
                  v
[Automated Welcome Inbound Trigger]
Business: "Hi Alex! Welcome to Apex Performance. To confirm you'd like to receive VIP drop alerts and order tracking via WhatsApp, please tap 'Confirm' below."
Buttons: [Confirm Opt-In] | [No Thanks]
                  |
                  v (Customer taps Confirm)
Business: "You're all set! Reply STOP anytime to pause messages. Here is your 15% VIP welcome code: APEX15."
```

---

## 3. Web Form Consent Copy (GDPR & TCPA Compliant)

```html
<label class="whatsapp-consent">
  <input type="checkbox" name="whatsapp_opt_in" required>
  <span>
    I agree to receive automated marketing and order update messages via WhatsApp from 
    <strong>[Brand Name]</strong> at the number provided. Consent is not a condition of purchase. 
    Message & data rates may apply. Reply STOP to cancel at any time. 
    View our <a href="/privacy">Privacy Policy</a>.
  </span>
</label>
```
