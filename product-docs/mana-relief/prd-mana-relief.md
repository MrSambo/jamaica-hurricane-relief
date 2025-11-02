# **Mana Relief Platform**

### **TL;DR**

Mana is a digital marketplace empowering international and Jamaican supporters to fund urgent hurricane relief by buying real items from trusted local suppliers—or via Amazon as fallback. The platform brings radical transparency and speed to giving, helping donors see their impact and strengthening Jamaica’s local recovery ecosystem.

---

## **Narrative**

In the aftermath of disaster, donors worldwide want to help, but are left wondering if their money does any good. Simultaneously, Jamaican businesses could meet urgent needs, yet often sit on the sidelines, disconnected from global generosity. Mana is the bridge: supporters directly fund relief items—from water to hygiene kits—which are then fulfilled by vetted local partners. Every contribution is visible, traceable, and delivers real value on the ground. By prioritizing local commerce and radical transparency, Mana creates trust and resilience now, while building capacity for the crises of tomorrow.

---

## **Success Metrics**

*Note: These are for internal direction, iteration, and learning only—not for restrictive performance targets due to the complexity of social impact work.*

### **User-Centric Metrics**

* Donor satisfaction score (surveyed post-donation)

* Percent of donors repeat-giving within 90 days

* Engagement time (on-site or via email updates)

### **Business Metrics**

* Value and percentage of purchases fulfilled by local suppliers

* Supplier retention and active participation rates

* Community/press testimonials, reputable partner endorsements

### **Technical Metrics**

* Platform uptime

* Median donation-to-fulfillment confirmation time

* Affiliate revenue generated for ops as a ratio to donations managed

### **Tracking Plan**

* Donation completion, supplier onboarding, fulfillment updates, donor feedback touchpoints

---

## **Goals**

### **Business Goals**

* Route >70% of funded goods through Jamaican suppliers

* Ship MVP within four weeks

* Onboard three reliable supplier partners and one NGO for launch

* Attach proof of fulfillment to every donation

### **User Goals**

* Supporters fund specific urgent needs, see proof, and can contribute easily

* Simple onboarding for vendors (no complex forms)

* Non-tech-savvy users participate confidently

### **Non-Goals**

* Mana does not own logistics or physical inventory

* No bespoke/perishable item purchases in MVP

* Not an official government entity or responsible for state-level infrastructure

---

## **User Stories**

**International Donor**

* As a diaspora supporter, I want to buy water or food for those in need, with confidence that a real local business will deliver.

**Local Supporter**

* As a resident, I want to contribute via mobile payment and see the direct outcome of my donation.

**Supplier/Business**

* As a local shop owner, I want to join Mana through a simple chat with an admin and get paid upon confirmed deliveries.

**Admin**

* As a coordinator, I want to update the relief needs list, verify suppliers, confirm fulfillment with photos, and keep donors informed.

---

## **Functional Requirements**

### **Relief Items Marketplace (High)**

* Dynamic, filterable catalog of needed goods (e.g., water, food, hygiene, hardware)

* Item card: name, urgency flag, detailed description, photo, progress bar, “Shop Local” and “Amazon” options, fulfillment progress—linked to transparency log

* Manual fulfillment workflow reference (see separate doc for details)

### **Donation & Payment (High)**

* Shop Local with in-platform checkout (Stripe/Donorbox, mobile wallet)

* Shop via Amazon: generates item/cart, supplies shipping/contact instructions, logs affiliate revenue

* Confirmation message and receipt with fulfillment tracking link

### **Supplier Directory & Onboarding (Medium)**

* Admin onboard of local suppliers by conversation (WhatsApp/email)

* Business doc upload (admin-facilitated) and supplier page

* Supplier catalog list view, filterable on backend

### **Transparency & Impact (High)**

* Feed of fulfilled items: order photo, timestamp, cost, item details

* Walls for donor testimonials and community response

* Validated press/partner logos where relevant

### **Admin Dashboard (Medium)**

* CRUD for item catalog & status

* Weekly order bundling, supplier comms, fulfillment/proof uploads

* Data export of donations, fulfillment, supplier list

### **Partnerships & Inquiry (Low)**

* Simple partnership contact form

* Admin workflow for vetting new NGOs/partners

---

## **User Experience**

**Entry Point & First-Time User Experience**

* Landing: clear call to see current relief needs

* Explainer content on how giving works, what’s urgent, and how impact is shown

**Core Experience**

* Donor selects item, chooses funding route, checks out, receives confirmation

* Admin bundles orders, coordinates via WhatsApp/email, uploads fulfillment; donors alerted when order is complete

* Supplier signs up via direct chat, verified by admin, updates maintained by admin as needed

**Reference:**  

See the “Mana Fulfillment Process” doc for granular fulfillment workflow and operational roles.

---

## **Technical Considerations**

Mana can be built as:

* **No-code/low-code MVP:** (Softr/Glide, Airtable, Donorbox/Stripe) for speed, lower cost, quick vendor onboarding

* **Custom-coded app:** (React/Node/etc.) for advanced automation, integrations, higher complexity/scale

This PRD does **not** mandate an approach: direction will reflect partners, resources, and platform learning.

**Core needs:**

* Modular backend (for payments, supplier data, fulfillment tracking), secure donor/admin access, privacy for payment data (third party held), and public transparency portal

* Security scaling as traffic/volume increases

---

## **Non-Technical Work & Challenges**

**Partnership Development:** Securing participation from reputable NGOs, government entities, and local organizations is foundational. This means dedicated outreach, ongoing communication, and careful vetting—both formal (due diligence, MOU) and informal (reference calls, community feedback).

**Supplier Engagement:** Local supplier onboarding requires face-to-face or conversational verification, local document checks, and establishing clear terms for order processing and payment. Ongoing relationship management is crucial—quality, timeliness, and communication standards must be reinforced, especially as volume grows.

**Legal, Compliance & Trust:** Navigating Jamaican and international legal landscapes for nonprofit partnerships, cross-border donations, tax exposure, affiliate income, and consumer protection takes proactive planning. All compliance needs must be clarified before go-live, with periodic review.

**Government Relations:** Partnering with ministries or agencies may be needed for bulk shipments, regulatory clearance, or data/reporting standards. Mana should be positioned as an asset—never an adversary or parallel authority.

**Public Narrative & Reputation:** Storytelling, transparent reporting, and proactive press/PR efforts are core to building trust and credibility—especially in disaster relief. Rapid response to misinformation or operational setbacks will be critical. Local community feedback and testimonials should be visible.

**On-the-Ground Operations:** Facilitating last-mile delivery requires partnerships with established couriers, distribution centers, or community orgs; ad-hoc logistics only works at very small scale. Documentation and process documentation for field operations are essential.

---

## **Milestones & Sequencing**

### **Project Estimate**

* MVP Build: 2–4 weeks

* Post-launch expansion: ongoing by priority

### **Team Size & Composition**

* 1–2 admin/operators

* 1 builder (no-code developer or web dev depending on platform path)

* 1 part-time partnerships/comms

### **Suggested Phases**

**Phase 1: Launch (2–4 weeks)**

* Live MVP, shop local/Amazon flow, admin dashboard, 1st suppliers, public impact feed

**Phase 2: Traction (1–2 months)**

* Expand partners, implement deeper reporting, integrate feedback, review for scale/custom dev

**Phase 3: Growth**

* Custom dev, advanced features, automation, expanded local reach as needed