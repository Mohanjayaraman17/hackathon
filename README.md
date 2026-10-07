# SmartSlot AI

> **Customer-Preferred Intelligent Delivery Slot Optimization**  
> *24-Hour Software Hackathon MVP*

---

## 🎯 Core Problem

When customers order products online, deliveries are traditionally scheduled according to the delivery company's convenience.

Customers may be:
- 🎓 In college lectures or lab sessions
- 💼 In office meetings
- 🚆 Commuting or travelling
- 🏠 Away from home during regular hours

**Example Scenario:**
> A student (Mohan) orders wireless headphones at 12:15 PM from his college campus in Pudukkottai. He is in lectures from 9:00 AM to 4:00 PM and is only free between 4:00 PM and 7:00 PM. In traditional delivery systems, the courier arrives whenever their route dictates—leading to missed parcels, re-attempt surcharges, and student frustration.

---

## 💡 The Main Innovation

**Traditional Delivery:**
```
Delivery chooses the time  ──►  Customer waits
```

**SmartSlot AI:**
```
Customer chooses available time  ──►  AI optimizes delivery to fit customer schedule
```

```
[CUSTOMER AVAILABILITY]
       │
       ▼
[PREFERRED DELIVERY SLOT]
       │
       ▼
[AI FEASIBILITY ANALYSIS] (Distance, Traffic, Rider Capacity, Delivery Load)
       │
       ▼
[SMART ALTERNATIVE RECOMMENDATION] (Peak shift optimization)
       │
       ▼
[SLOT CONFIRMATION & ON-TIME HANDOVER] (96% probability)
```

> **Core Presentation Motto:**  
> *"Customers shouldn't have to change their schedule for delivery. SmartSlot AI makes delivery fit the customer's schedule."*

---

## 🛠️ Technology Stack

- **Frontend:** HTML5, CSS3, Modern Vanilla JavaScript (ES6+)
- **Visual Analytics:** Chart.js (Loaded via CDN)
- **Data Persistence:** Browser `localStorage` (Preserves demo data across page reloads)
- **Zero Heavy Frameworks:** Pure, lightning-fast client architecture runnable directly in any browser.

---

## 🚀 Key Features & Flow

### 1. Landing Page (`#landing`)
- Premium dark interface with electric blue and cyan neon accents.
- End-to-end visual flow and direct comparison cards between traditional vs. SmartSlot AI delivery models.
- Highlighting core product value proposition.

### 2. Place Order (`#order`)
- Pre-configured product catalog presets (Wireless Headphones, Ergonomic Laptop Stand, Smartwatch, Textbooks).
- Inputs for Product Name, Price, Delivery Address (Pudukkottai Campus), Delivery Area, and Date.

### 3. Customer Availability (`#availability`)
- Preset selection: Morning, Afternoon, Evening, and Custom Availability.
- Interactive **Visual Schedule Timeline (8 AM – 9 PM)** mapping unavailable vs. free handover hours.
- Dynamic slot compatibility tagging based on customer schedule.

### 4. Select Delivery Slot (`#slots`)
- Eight operational slots:
  - `8–10 AM` (AVAILABLE)
  - `10–12 PM` (LIMITED)
  - `12–2 PM` (FULL)
  - `2–4 PM` (LIMITED)
  - `4–5 PM` (HIGH DEMAND — Peak student rush)
  - `5–6 PM` (AVAILABLE — AI Recommended Sweet Spot)
  - `6–7 PM` (AVAILABLE)
  - `7–9 PM` (LIMITED)

### 5. Deterministic AI Feasibility Engine (`#analysis`)
Evaluates 6 physical and spatial constraint factors using deterministic JavaScript mathematical scoring (Starting base 100):
1. **Dispatch Distance:** 7.8 km from central fulfillment hub.
2. **Traffic Congestion Index:** Medium / High / Low.
3. **Delivery Load Factor:** Sector queue volume (e.g., 82%).
4. **Rider Fleet Availability:** Active couriers in proximity.
5. **Area Cluster Demand:** Surge status in the target drop zone.
6. **Customer Window Overlap:** Verifies alignment with available hours.

Calculates:
- **Slot Score:** 0 to 100
- **On-Time Probability:** (e.g., 68% vs 96%)
- **Delay Risk:** Low / Medium / High
- **Confidence Metric:** ~94–97%

### 6. Smart Alternative Recommendation (`#recommendation`)
- Flags bottlenecks in requested high-demand slots (e.g., 4:00 PM – 5:00 PM).
- Recommends the optimal slot (5:00 PM – 6:00 PM) that maintains high on-time delivery while staying strictly within the customer's free window.
- Provides choices: `Accept Recommended Slot` or `Keep My Original Slot`.

### 7. Slot Confirmation (`#confirmation`)
- Summary screen displaying verified handover window, ETA, on-time certainty, and dispatch parameters.

### 8. Real-Time Delivery Tracking (`#tracking`)
- 5-stage milestone stepper (`Order Confirmed` ➔ `Packed` ➔ `Delivery Partner Assigned` ➔ `Out for Delivery` ➔ `Delivered`).
- Assigned rider details: Arun (4.9★ rating, Electric Scooter).
- Distance remaining (2.8 km) and accurate estimated arrival (5:32 PM).

### 9. Operations Dashboard (`#dashboard`)
- 5 key logistics KPIs: Total Orders (128+), Confirmed Slots (94+), On-Time Rate (91%), Active Deliveries (18), High-Demand Slots (3).
- **Chart 1:** Delivery Demand by Hour (Bar chart).
- **Chart 2:** Slot Capacity Utilization (Doughnut chart).
- **Chart 3:** On-Time Delivery Rate: Traditional (68%) vs SmartSlot AI (96%).
- Live order history table synced to `localStorage`.

### 10. Automated Live Hackathon Demo
- Click **"⚡ RUN LIVE DEMO"** in the top bar.
- Runs an automated 35–45 second scenario demonstrating Mohan's college order flow with narrated judge milestones.

---

## 🏃‍♂️ How to Run

### Option 1: Open Directly in Browser
Double-click `index.html` or open via browser:
```bash
# On Linux / Mac / Windows
open index.html
```

### Option 2: Run via Node Dev Server
```bash
npm run dev
```
The application will launch at `http://localhost:3000`.

---

## 🏆 24-Hour Scope Discipline
Designed strictly around the hackathon problem statement:
- ✅ Focus on customer availability & constraint optimization.
- 🚫 Excludes unnecessary production bloat (payments, external GPS hardware, microservices, complex cloud dependencies).
