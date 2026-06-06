🚀 Performance Testing of Restful-Booker API using Apache JMeter
________________________________________
📌 Project Overview
This project demonstrates performance testing of the Restful-Booker API using Apache JMeter (5.6.3).
The main objective is to evaluate the API’s:
•	⚡ Responsiveness 
•	🛡️ Stability 
•	🔄 Reliability under concurrent user load 
________________________________________
🛠️ Testing Tool
•	Apache JMeter 5.6.3 
________________________________________
🌐 Test Environment
Parameter		Value
Tool		Apache JMeter 5.6.3
Virtual Users (Threads)		10
Ramp-Up Time		1 Second
Loop Count		1
Error Rate		0%
________________________________________
📡 Tested API Endpoints
The following endpoints were tested during performance execution:
•	📥 Get Booking IDs 
•	➕ Create Booking 
•	🔍 Get Booking Details 
•	🔐 Create Authentication Token 
•	✏️ Update Booking 
________________________________________
🎯 Test Scenario
The test simulates 10 concurrent users accessing the API simultaneously.
⚙️ Configuration Summary
•	👥 Users: 10 Threads 
•	⏱️ Ramp-Up: 1 Second 
•	🔁 Loop Count: 1 
•	⏲️ Constant Timer: Added between requests 
•	📊 Listener: Summary Report 
•	🔍 Validation: View Results Tree 
________________________________________
🔄 Test Flow
Get Booking IDs
      ↓
Create Booking
      ↓
Get Booking
      ↓
Create Token
      ↓
Update Booking
      ↓
Verify Updated Booking
________________________________________



🧱 JMeter Test Plan Structure
Test Plan
│
└── Thread Group
    │
    ├── GetBookingIds
    │   ├── HTTP Request
    │   └── Constant Timer
    │
    ├── CreateBooking
    │   ├── HTTP Request
    │   └── Constant Timer
    │
    ├── GetBooking
    │   ├── HTTP Request
    │   └── Constant Timer
    │
    ├── CreateToken
    │   ├── HTTP Request
    │   └── Constant Timer
    │
    ├── UpdateBooking
    │   ├── HTTP Request
    │   └── Constant Timer
    │
    ├── VerifyUpdatedBooking
    │
    ├── View Results Tree
    └── Summary Report
________________________________________
📊 Test Results Summary
Metric	Result
👥 Concurrent Users	10
⏱️ Ramp-Up Time	1 Second
❌ Total Errors	0
📉 Error Rate	0%
🌐 API Availability	100%
✅ Test Status	Passed
________________________________________


📈 Key Findings
✅ All API endpoints responded successfully under load
✅ No request failures detected
✅ Authentication worked smoothly under concurrent access
✅ Booking CRUD operations remained stable
✅ System handled load without performance degradation
✅ Overall execution result: 100% success rate
________________________________________
📷 Screenshots
🧪 JMeter Test Plan


📊 Summary Report
 

📈 View Results Tree
 
________________________________________
📂 Repository Structure
Performance-Testing-RestfulBooker/
│
├── Test Plan/
│   └── Project2.jmx
│
├── Screenshots/
│   ├── jmeter-test-plan.png
│   ├── summary-report.png
│   └── view-results-tree.png
│
├── Reports/
│   └── performance-report.png
│
└── README.md
________________________________________
🏁 Conclusion
The Restful-Booker API performance testing was successfully executed using Apache JMeter.
Under a load of 10 concurrent users with 1-second ramp-up, the API:
•	Performed consistently ⚡ 
•	Showed no failures ❌ 
•	Maintained stability 🛡️ 
•	Achieved 100% success rate 🎯 

