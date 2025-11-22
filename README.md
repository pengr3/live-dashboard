# CLMC Operations Dashboard

**Real-time Facility Management & Maintenance Analytics Dashboard**

Connected to live Google Sheets data for tracking maintenance operations, repairs, inspections, and equipment inventory.

---

## 🚀 Quick Start

### **Step 1: Download the Dashboard**
1. Download `dashboard.html` file
2. That's it! It's a single-file application.

### **Step 2: Access the Dashboard**

**Option A: Open Locally (Immediate)**
- Double-click `dashboard.html` to open in your browser
- Login with password: `clmc2024`

**Option B: Deploy to GitHub Pages (Recommended for Team Access)**
See deployment instructions below.

---

## 🔐 Authentication

**Default Password:** `clmc2024`

**To Change Password:**
1. Open `dashboard.html` in a text editor
2. Find line: `PASSWORD: 'clmc2024'`
3. Change to your desired password
4. Save the file

---

## 📊 Dashboard Features

### **1. Calendar View**
- Visual timeline of all completed work orders
- Scheduled maintenance due dates
- Color-coded by client (Blue = Stefanini, Green = PPHI)
- Click any event for detailed information

### **2. Key Metrics Cards**
- ✅ **Maintenance Projects** - Total completed maintenance tasks
- 🔨 **Repairs** - Total repair work orders
- 📋 **Inspections** - Total inspection tasks
- Trend indicators vs. previous period

### **3. Date Range Filtering**
- Custom date range selector
- Quick filters: This Week, This Month, This Quarter, This Year
- All metrics and calendar update dynamically

### **4. Client Performance Dashboard**
- Bar chart showing projects by client
- Equipment distribution analysis

### **5. Equipment Analytics**
- Equipment type breakdown (HVAC, FDAS, Pest Control, Disinfection)
- Visual doughnut chart

### **6. Upcoming Maintenance (Next 30 Days)**
- List of equipment due for maintenance
- Days remaining countdown
- Sorted by urgency

### **7. Overdue Equipment Alerts**
- Critical overdue items
- Days overdue tracking
- Prioritized list

### **8. PDF Export**
- Generate printable reports
- Includes all key metrics
- Date-stamped for records

---

## 🔄 Live Data Connection

**The dashboard automatically pulls data from:**
- Google Sheets ID: `1tOgX3dpNJepbe6GERLjmWwvEOSU3UetybRxtGoogdcY`

**Sheets Connected:**
1. WorkOrders - Completed maintenance/repair/inspection tasks
2. Inventory - Equipment list with due dates and maintenance schedules
3. Report_Delivery_Log - Service report delivery tracking
4. Reminders_Logs - Equipment reminder notifications

**Data Refresh:**
- Click "🔄 Refresh" button to pull latest data
- Automatic refresh every time you reload the page

---

## 🌐 Deploying to GitHub Pages (Team Access)

### **Step 1: Create GitHub Repository**
```bash
# In your terminal/command prompt:
cd /path/to/your/folder
git init
git add dashboard.html
git add README.md
git commit -m "Initial CLMC Dashboard"
```

### **Step 2: Push to GitHub**
```bash
# Create a new repository on GitHub.com, then:
git remote add origin https://github.com/YOUR-USERNAME/clmc-dashboard.git
git branch -M main
git push -u origin main
```

### **Step 3: Enable GitHub Pages**
1. Go to your repository on GitHub.com
2. Click "Settings" tab
3. Scroll to "Pages" section (left sidebar)
4. Under "Source", select "main" branch
5. Click "Save"
6. Your dashboard will be live at: `https://YOUR-USERNAME.github.io/clmc-dashboard/dashboard.html`

---

## 📱 Mobile Access

The dashboard is fully responsive and works on:
- ✅ Desktop computers
- ✅ Tablets
- ✅ Mobile phones

---

## 🛠️ Technical Details

**Built With:**
- Vanilla JavaScript (no complex build process needed)
- FullCalendar.js - Calendar visualization
- Chart.js - Charts and graphs
- Tailwind CSS - Styling
- Google Sheets API - Live data connection

**Browser Compatibility:**
- Chrome ✅
- Firefox ✅
- Safari ✅
- Edge ✅

---

## 🔧 Customization

### **Change Client Colors**
Edit the `CLIENT_COLORS` object in the code:
```javascript
const CLIENT_COLORS = {
    'Stefanini': '#3B82F6',  // Blue
    'PPHI': '#10B981',       // Green
    'Default': '#8B5CF6'     // Purple
};
```

### **Add More Clients**
Simply add them to the `CLIENT_COLORS` mapping with hex color codes.

### **Modify Date Ranges**
Adjust the quick filter periods in the `setQuickFilter()` function.

---

## 📞 Support & Troubleshooting

### **Common Issues:**

**Problem: "Error loading data"**
- ✅ Check internet connection
- ✅ Verify Google Sheets is shared properly (Anyone with link can view)
- ✅ Check browser console for specific errors (F12)

**Problem: "Calendar not showing events"**
- ✅ Verify WorkOrders sheet has CompletionDate data
- ✅ Check date format is MM/DD/YYYY
- ✅ Try clicking "Refresh" button

**Problem: "Charts not displaying"**
- ✅ Clear browser cache
- ✅ Try different browser
- ✅ Check if data exists in filtered date range

---

## 📈 Future Enhancements

Possible additions:
- Email notifications for overdue equipment
- Personnel workload analysis
- Cost tracking and budget reports
- Location-based heatmaps
- Automated weekly reports
- Mobile app version

---

## 📄 License

Internal use for CLMC operations team.

---

## 👨‍💻 Developer

Built by Francis Silva  
CLMC n8n Automation Expert  
Contact: pengr.clmc.3@gmail.com

---

**Last Updated:** November 21, 2025  
**Version:** 1.0.0
