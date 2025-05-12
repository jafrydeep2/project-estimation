# TapOrder – 3-Month MVP Development Plan (Budget: $8,000)

## Month 1 – UI/UX Design + Backend Setup
**Budget: $2,000**

### Week 1 – Planning & Wireframes
- Finalize key user flows: Customer, Waiter, Manager
- Create low-fidelity wireframes:
  - Customer App
  - Waiter Dashboard
  - Manager Panel

### Week 2 – UI Design
- Design high-fidelity UI screens:
  - Welcome Screen
  - Menu & Cart
  - Payment & Confirmation
  - Live Orders (Waiter)
  - Manager Overview Page

### Week 3–4 – Backend Setup
- Design database schema (users, tables, orders, menu)
- Set up backend framework (Node.js / Django)
- Create basic REST APIs:
  - Auth & Role Management
  - Order Placement
  - Menu Retrieval
  - Table/NFC Mapping

---

## Month 2 – Frontend + Backend Core
**Budget: $3,000**

### Week 1–2 – Customer Web App
- Implement NFC scan flow (detect table number)
- Build digital menu with categories and images
- Add-to-cart functionality with notes
- Sticky cart with quantity edit & removal
- Stripe payment gateway integration

### Week 3–4 – Backend Core Functionality
- Connect frontend with backend APIs
- Store and forward order to POS (mock/integration-ready)
- Handle order status logic (Received, In Progress, Ready)
- Enable real-time updates via polling or WebSocket

---

## Month 3 – Staff Panels + QA & Launch
**Budget: $3,000**

### Week 1 – Waiter Dashboard
- Display live orders by table number
- View item details and special notes
- Update order status with color codes
- Sound/visual alerts for new orders

### Week 2 – Restaurant Manager View
- View all orders with basic analytics
- Menu editor (add/edit/delete items)
- Control availability and pricing

### Week 3 – Super Admin Panel
- Manage restaurant accounts and credentials
- Monitor system errors and POS status
- View subscription status (manual)

### Week 4 – QA & Final Launch
- Cross-device browser testing (mobile, tablet)
- Validate payment and order flows
- Bug fixing and final polish
- Launch to production or staging environment

---

## Summary Table

| Phase                     | Key Tasks                                            | Timeline        | Budget   |
|--------------------------|------------------------------------------------------|-----------------|----------|
| UI/UX Design             | Wireframes, UI design                                | Month 1 (W1–2)  | $1,000   |
| Backend Setup            | Schema, API structure                                | Month 1 (W3–4)  | $1,000   |
| Customer App             | Menu, cart, payment                                  | Month 2 (W1–2)  | $1,500   |
| Backend Core             | Order flow, POS connection                           | Month 2 (W3–4)  | $1,500   |
| Waiter & Manager Panels  | Live view, menu mgmt, dashboards                     | Month 3 (W1–2)  | $1,500   |
| Super Admin + QA         | Admin panel, testing, launch                         | Month 3 (W3–4)  | $1,500   |

**Total Duration:** 3 Months  
**Total Budget:** $8,000  
**Outcome:** Lean, production-ready MVP
