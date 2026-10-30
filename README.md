# 🎓 CADHS Institute of Engineering (CADHS)
## B.Tech Centralized College Admission System (Academic Year 2026-2027)

A complete, modern, responsive web application for managing Bachelor of Technology (B.Tech) admissions, student registration, eligibility calculation, fee estimation, multi-channel payment processing, and automatic email dispatching.

---

## 🌟 Key Features Implemented

### 1. Student Registration Wizard
* **Multi-Step Guided Flow**:
  - **Step 1: Student Profile**: Full Name, Student Email Address, 10-digit Mobile Number, Date of Birth, Gender (with Girl Child Grant), Quota Category (General, OBC-NCL, SC, ST, EWS), Guardian Details, and Residential Address.
  - **Step 2: Academic Qualifications**:
    - **10th Grade Marks**: Board, School Name, Passing Year, Roll No, Marks Obtained vs Max Marks with **Instant Auto Percentage Calculation**.
    - **12th Grade Marks**: Board, School, Passing Year, and individual subject marks for **Physics, Chemistry, and Mathematics (PCM)** + Optional Subject (CS / English).
    - **PCM Aggregate Calculation**: Automatically computes your 12th PCM aggregate percentage out of 300, which is the statutory engineering benchmark.
    - **Entrance Examination**: JEE Main percentile / State CET Rank and admit card roll number.
  - **Step 3: B.Tech Course Selection**:
    - Select 1st, 2nd, and 3rd Engineering branch preferences.
    - Choose on-campus Hostel & Accommodation options (Day Scholar, AC, Non-AC Double/Single room with 4-meal mess).
    - **Live Eligibility Status Indicator**: Evaluates whether the student's 10th and 12th PCM marks meet the cutoff for their selected engineering branch.
  - **Step 4: Fees Breakdown & Payment Gateway**:
    - Transparent fee breakdown with automatic merit scholarship deduction based on 12th PCM marks.
    - Choose payment type: **Seat Booking Token (₹25,000)**, **Full 1st Semester Fee (₹87,500)**, or **Application Processing Fee (₹1,200)**.
    - Select Payment Method: UPI QR Code, UPI ID (VPA), Credit/Debit Card, or Net Banking.
    - Simulated 256-bit SSL banking authorization progress.

---

### 2. B.Tech Engineering Course Catalog
Includes 8 approved undergraduate disciplines:
1. **B.Tech Computer Science & Engineering (CSE)** - 180 Seats
2. **B.Tech CSE (Artificial Intelligence & Machine Learning)** - 120 Seats
3. **B.Tech CSE (Data Science & Analytics)** - 60 Seats
4. **B.Tech Electronics & Communication Engineering (ECE)** - 120 Seats
5. **B.Tech Information Technology (IT)** - 120 Seats
6. **B.Tech Electrical & Electronics Engineering (EEE)** - 60 Seats
7. **B.Tech Mechanical Engineering (Robotics & Mechatronics)** - 60 Seats
8. **B.Tech Civil & Smart Infrastructure Engineering** - 60 Seats

Each course card displays approved intake, duration, minimum 10th %, minimum 12th PCM %, JEE cutoffs, average placement package, and annual tuition fee.

---

### 3. Selection Criteria Framework & Interactive Cutoff Engine
* **Statutory Minimums**: AICTE & University baseline (min 45% in 12th PCM, 40% for reserved category).
* **Branch Cutoff Table**: Clear benchmark cutoffs for all 8 branches.
* **Interactive "Instant Eligibility Evaluator"**: Enter your 10th %, 12th PCM %, and entrance score to immediately see which engineering programs you qualify for:
  - 🟢 **Direct Merit Eligible**
  - 🟡 **Counseling / CAP Round Eligible**
  - 🔴 **Below Benchmark / Alternate Branch Recommended**
* **Scholarship Schemes**:
  - *Chairman's Super Merit*: 50% Tuition Waiver for 12th PCM >= 95%
  - *Merit Excellence*: 25% Tuition Waiver for 12th PCM 90% - 94.9%
  - *STEM Talents*: 10% Tuition Waiver for 12th PCM 85% - 89.9%
  - *Girl Child in Engineering*: Additional ₹15,000 scholarship

---

### 4. Transparent Fees Structure & Dynamic Calculator
* Itemized fee table for all 4 years:
  - Tuition Fee (Instructional & Faculty)
  - Laboratory & Computing Facility Kit
  - Examination & University Affiliation
  - Digital Library, IEEE Journals & Tech Subscriptions
  - Sports, Gymkhana & Cultural Development Fund
  - Student Medical Insurance
  - One-time Refundable Caution Deposit (₹10,000)
* **Interactive Fee Estimator**: Select course, hostel option, and 12th PCM % to dynamically calculate net payable amount and semester installment.

---

### 5. Multi-Option Payment Gateway
* **UPI / QR Code**: Dynamic QR code with live scanning beam, 5-minute security countdown, and UPI VPA verifier.
* **Credit / Debit Cards**: Card number input with auto-formatting, cardholder name, expiry, CVV, and mock 3D-Secure authentication.
* **Net Banking**: Direct gateway integration mock for State Bank of India, HDFC Bank, ICICI Bank, and Axis Bank.

---

### 6. Automated Email Notification System
* **Triggered Immediately Upon Payment**:
  - System generates a formal digital admission confirmation and payment acknowledgment.
  - Dispatches email to the student's registered email address.
  - Floating **"Email Inbox"** drawer button in the navigation bar with unread count badge.
  - **Simulated Student Email Client**:
    - Sender: `CADHS Institute Admissions <admissions@cadhs-eng.edu.in>`
    - To: Candidate's registered email address
    - Subject: `🎉 Admission Payment Successful & Provisional Confirmation - [App No: CADHS-2026-XXXX]`
    - Body: Formal letterhead, candidate academic scores, provisional seat allotment, transaction receipt voucher, document verification venue, and Dean's electronic signature.
    - Options to print, re-send, or save.

---

### 7. Student Dashboard & Application Tracking
* Search by Application ID (e.g. `CADHS-2026-0814`) or registered student email.
* Displays 4-step progress timeline: Registered ➔ Criteria Verified ➔ Fee Paid ➔ Verification Due.
* View and print:
  - **Formal Fee Receipt (PDF / Print-friendly)**
  - **Provisional Seat Allotment Letter**

---

### 8. Admissions Office & Staff Desk
* Real-time metrics: Total Registered Candidates, Paid Seats, and Total Fees Collected.
* Comprehensive applicant directory with branch filters and mark breakdowns.
* **Export to CSV**: Export all student admissions data to Excel/CSV with one click.

---

## 🚀 How to Run the Website

### Option 1: Double-click to Run Local Server
Simply double-click the included `start.bat` file in the project folder. It will launch the local HTTP server at:
👉 **`http://localhost:3000`**

### Option 2: Using Command Line (Node.js)
```bash
cd "C:\Users\chetan shelar\.gemini\antigravity\scratch\college-admission-system"
node server.js
```
Then open your web browser and navigate to:
`http://localhost:3000`

### Option 3: Direct Browser Launch (Zero Dependencies)
You can also open the `public/index.html` file directly in Google Chrome, Microsoft Edge, or Mozilla Firefox! All client-side storage, calculations, eligibility tests, payment simulations, and email mock drawers work seamlessly offline via `localStorage`.

---

## 📁 Project Directory Structure

```
college-admission-system/
├── public/
│   ├── index.html        # Complete responsive web application
│   ├── styles.css        # Custom aesthetic CSS, animations, and print media rules
│   ├── app.js            # Frontend state, wizard logic, payment gateway & email engine
│   └── data.js           # Courses catalog, selection criteria rules & seed data
├── data/
│   ├── applications.json # Persistent applications file store
│   └── emails.json       # Persistent dispatched emails log
├── server.js             # Built-in Node.js HTTP & REST API server
├── package.json          # Package configuration and scripts
├── start.bat             # Windows one-click server starter
└── README.md             # Complete user guide and system documentation
```
