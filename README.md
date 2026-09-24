# Registration-Form-Midterm

Interactive Student Registration Form built with **React** and **Vite** for the University of Caloocan City (UCC).

## ✨ Features

- **Personal Information**:
  - First Name, Last Name (letters only, 2–50 chars, no spaces)
  - Middle Initial / Name (Optional: supports single letter initial like `S` or full middle name like `Santos`)
- **Birthdate Validation**:
  - Dynamic Month, Day, and Year dropdowns (up to 2026)
  - Accurate calendar limits: February limited to 28/29 days with leap-year awareness, 30 days for 30-day months, 31 days for others
  - Live age calculation and formatted `mm/dd/yy` system date display
- **Philippine Holidays Lookup**:
  - Standalone Year dropdown (up to 2026) that automatically renders all Regular and Special Philippine holidays for the selected year
- **3-Tier Address Hierarchy**:
  - No. of Block / Street input
  - Cascading dropdowns: Region (all 17 PH regions) → City → Barangay
  - 100% accurate Caloocan City Barangay 176 support (RA 11993 176-A through 176-F and resident Phases 1 to 10 including UCC Engineering Phase 8-A)
- **Security & Validation**:
  - Password strength validation (8+ chars, upper, lower, number, special char)
  - Password visibility toggle & confirm password real-time verification
- **Verified Registration Preview**:
  - Clean preview table of all submitted information upon submission

## 🚀 Getting Started

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

