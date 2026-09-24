# Registration-Form-Midterm

Interactive Student Registration Form built with React and Vite for the University of Caloocan City (UCC).

## Features

- **Personal Information**:
  - First Name, Last Name (letters only, 2–50 chars, no spaces)
  - Middle Initial / Name (Optional: supports single letter initial like `S` or full middle name like `Santos`)
- **Live Email Domain API Verification**:
  - Validates email format and verifies domain existence in real-time using Google Public DNS over HTTPS (with Cloudflare DoH fallback)
  - Resolves MX (Mail Exchange) and A records without hardcoded domain lists
- **Birthdate Validation**:
  - Dynamic Month, Day, and Year dropdowns (up to 2026)
  - Accurate calendar limits: February limited to 28/29 days with leap-year awareness, 30 days for 30-day months, 31 days for others
  - Live age calculation and formatted `mm/dd/yy` system date display
- **Philippine Holidays Lookup**:
  - Standalone Year dropdown (up to 2026) that automatically renders all Regular and Special Philippine holidays for the selected year without extra selection
- **Philippine Standard Geographic Code (PSGC) API Integration**:
  - Live public API integration (`https://psgc.gitlab.io/api/`) covering all 17 Philippine Regions, 1,634+ Cities/Municipalities, and 42,000+ Barangays nationwide
  - Cascading dropdowns: Region -> City / Municipality -> Barangay with dynamic counts and loading feedback
  - 100% accurate Caloocan City Barangay 176 support (Republic Act No. 11993: Barangays 176-A to 176-F, resident Phases 1 to 10 including UCC Engineering Campus Phase 8-A, and named districts)
  - Built-in caching and offline fallback for continuous resilience
- **Security & Live Real-Time Validation**:
  - Real-time password criteria checklist (8+ chars, upper, lower, number, special char)
  - Password visibility toggle and confirm password verification
  - Real-time live registration status banner (no submit button required)
- **Live Registration Preview**:
  - Clean preview table updating in real time as the user types and selects

## Getting Started

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```
