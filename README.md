# SMART-ECOSPHERE

## 1. Project Overview & Inspiration

Modern households strive to adopt sustainable habits, but managing domestic micro-waste, energy budgets, and inventory rotation often feels fragmented. **Smart EcoSphere** is an all-in-one household sustainability operating system designed to transform daily domestic choices into verified environmental impact.

By pairing zero-cloud client privacy with automated tools—such as OCR receipt extraction, First-In-First-Out (FIFO) food rotation, appliance telemetry modeling, and AI recipe generation—Smart EcoSphere empowers users to track and optimize their ecological footprint effortlessly.

---

## 2. Core Functional Modules

### 🍏 FreshVault Inventory (Perishables)
- **Objective:** Mitigate kitchen spoilage by tracking expiration timelines for perishable items.
- **Key Functionality:** Logs purchase dates, computes remaining shelf life, and dynamically flags items expiring within a 3-day window to prioritize consumption.

### 📦 PantryFIFO (Staples Management)
- **Objective:** Enforce First-In, First-Out inventory rotation for non-perishable goods.
- **Key Functionality:** Tracks bulk staples (rice, grain, legumes), monitors minimum threshold levels, and prompts restocking only when reserves dip below defined limits.

### ⚡ WattWatch Energy Calculator & Smart AC Automation
- **Objective:** Quantify appliance power draw and model energy-saving scenarios.
- **Key Functionality:** Computes monthly kilowatt-hour ($\text{kWh}$) consumption and utility bills ($\text{₹}$) using custom tariff rates. Integrates a **Smart Cooling Automation** routine that syncs with Bluetooth temperature sensors to trigger AC cutoffs and smart home (Alexa) routines upon reaching target room temperatures.

### 🍳 RescueChef AI
- **Objective:** Convert near-expiry ingredients into culinary meals rather than landfill waste.
- **Key Functionality:** Automatically extracts high-priority items from **FreshVault**, accepts additional leftover inputs (`e.g., rice, dal, bread`), and generates zero-waste meal suggestions.

### 🧾 Smart Receipt Scan
- **Objective:** Streamline data entry via automated document parsing.
- **Key Functionality:** Accepts uploaded grocery receipts ($\text{PDF}, \text{JPG}, \text{PNG}, \text{WEBP}$) and applies browser-based OCR text extraction to populate pantry tables with a single click.

---

## 3. Impact Calculation Methodology

Smart EcoSphere evaluates aggregate household climate mitigation using a unified carbon-equivalent formula:

$$ \text{CO}_2\text{e Avoided (kg)} = (M_{\text{fresh}} \times 2.5) + (M_{\text{pantry}} \times 1.8) + \left[ (E_{\text{baseline}} - E_{\text{actual}}) \times 0.85 \right] $$

Where:
- \( M_{\text{fresh}} \) = Mass of perishable food saved from waste (\text{kg})
- \( M_{\text{pantry}} \) = Mass of pantry staples rotated via FIFO (\text{kg})
- \( E_{\text{baseline}} \) = Standard expected appliance energy consumption (\text{kWh})
- \( E_{\text{actual}} \) = Optimized household consumption (\text{kWh})

---


```
