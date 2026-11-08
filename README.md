# Mariam Electronics Store - Daily Sales Record
## Built From Scratch in Excel

## 📋 Project Overview
Built a complete Daily Sales Record system from scratch for Mariam Electronics Store - no downloaded data, everything created by me.

## 🏪 What I Built From Scratch
1. **List Sheet (Lookup Tables)**
   - Category Code: Laptop = LP, Phone = PH, WhiteGoods = WG, TV = TV
   - State Code: Abuja = ABJ, Lagos = LAG, Rivers = RWS
   - LGA Code: Abaji = AB, Gwagwalada = GW, Kuje = KU, Epe = EP, Agege = AG, Alimosho = AL, Port Harcourt = PH, Akpor = AK, Eleme = EL
   - Sales Rep: Chinedu, Dami, Olu, Zainab
   - LGA to Location lists: Naharati Layout, Sabon-Tash, Phase 1 Market, etc.

2. **Name Manager**
   - Named every table as a Named Range: CategoryCode, StateCode, LGACode, CATEGORY, STATE, LGA, Customer, Laptop, TV, Phone, etc.
   - So formulas can use clean names instead of cell addresses.

3. **Sales Sheet - Daily Sales Record**
   Columns: S/N | Date | Customer Name | Transaction ID | Category | Sub-Category | Product Name | Qty | Unit Price | Sales | State | LGA | Location | Sales Rep
   - Dropdowns (Data Validation) for Category, Sub-Category, Product, State, LGA
   - Transaction ID auto-generated from codes
   - Sales = Qty * Unit Price

4. **Customer Sheet**
   - Customer list linked to Sales sheet

## 🧠 Key Formulas Used
- Location:
  =VLOOKUP(Category, CategoryCode, 2, FALSE) & "/" & MID(...) & VLOOKUP(State, StateCode, 2, FALSE) & "/" & VLOOKUP(LGA, LGACode, 2, FALSE)
- VLOOKUP to pull codes from List sheet
- MID to extract parts of Transaction ID

## 🛠️ Tools Used
- Microsoft Excel
- Data Validation (Dropdowns)
- Name Manager / Named Ranges
- VLOOKUP, MID

## 📊 Result
A full working sales system - type Customer, pick Category / State / LGA, and Transaction ID, Sales and Location fill automatically. Clean, fast, no manual typing errors.

## 📂 Files in this Repo
- Mariam_Electronics_Store.xlsx

---
*Created from scratch by Mariam44*
