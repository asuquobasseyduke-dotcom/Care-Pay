<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Care Roster & Pay Calculator</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            orchardPurple: '#4B2A68',
            orchardDark: '#2D193F',
            orchardCard: '#3B2153',
            orchardNavy: '#1E2538',
            orchardTeal: '#00A699',
            colorDS: '#2563EB',
            colorWN: '#0D9488',
            colorSO: '#7C3AED',
            colorTr: '#EA580C'
          }
        }
      }
    }
  </script>
</head>
<body class="bg-slate-100 font-sans min-h-screen pb-12">

  <!-- Header -->
  <header class="bg-orchardPurple text-white py-6 px-4 text-center shadow-md">
    <h1 class="text-2xl font-bold tracking-tight">Personal Roster Calculator</h1>
    <p class="text-xs text-purple-200 mt-1">Private Financial Estimation Tool</p>
  </header>

  <main class="max-w-xl mx-auto px-4 mt-6 space-y-6">

    <!-- Payday Card 1 -->
    <div class="bg-orchardPurple text-white p-5 rounded-2xl shadow-lg border border-purple-900/30">
      <p class="text-xs uppercase tracking-wider text-purple-200 font-semibold">Next Immediate Payday</p>
      <p id="nextPaydayDate" class="text-xl font-bold mt-1">Thursday 6 August 2026</p>
      <p id="nextPaydayPeriod" class="text-xs text-purple-300 mt-0.5">Period: 13 Jul to 26 Jul</p>
      
      <div class="border-t border-purple-400/20 my-3"></div>
      
      <div class="flex justify-between items-center text-sm">
        <div>
          <span class="text-xs text-purple-300 block">Gross Estimate</span>
          <span id="nextPaydayGross" class="font-bold text-lg">€0.00</span>
        </div>
        <div class="text-right">
          <span class="text-xs text-purple-300 block">Net (Est.)</span>
          <span id="nextPaydayNet" class="font-bold text-lg text-emerald-300">€0.00</span>
        </div>
      </div>
    </div>

    <!-- Payday Card 2 -->
    <div class="bg-orchardNavy text-white p-5 rounded-2xl shadow-lg border border-slate-800">
      <p class="text-xs uppercase tracking-wider text-slate-400 font-semibold">Following Payday</p>
      <p id="followingPaydayDate" class="text-xl font-bold mt-1">Thursday 20 August 2026</p>
      <p id="followingPaydayPeriod" class="text-xs text-slate-400 mt-0.5">Period: 27 Jul to 9 Aug</p>
      
      <div class="border-t border-slate-700/50 my-3"></div>
      
      <div class="flex justify-between items-center text-sm">
        <div>
          <span class="text-xs text-slate-400 block">Gross Estimate</span>
          <span id="followingPaydayGross" class="font-bold text-lg">€0.00</span>
        </div>
        <div class="text-right">
          <span class="text-xs text-slate-400 block">Net (Est.)</span>
          <span id="followingPaydayNet" class="font-bold text-lg text-teal-300">€0.00</span>
        </div>
      </div>
    </div>

    <!-- Calendar Section -->
    <div class="bg-white p-5 rounded-2xl shadow-md border border-slate-200">
      
      <!-- Month/Year Selection & Header Controls -->
      <div class="flex flex-wrap items-center justify-between gap-2 mb-4 pb-3 border-b border-slate-100">
        
        <!-- Dropdown selectors for 12 months & years -->
        <div class="flex items-center gap-2">
          <select id="monthSelect" onchange="changeCalendarView()" class="bg-slate-100 font-bold text-slate-800 text-sm py-1.5 px-2.5 rounded-lg border border-slate-300 outline-none focus:ring-2 focus:ring-purple-600">
            <option value="0">January</option>
            <option value="1">February</option>
            <option value="2">March</option>
            <option value="3">April</option>
            <option value="4">May</option>
            <option value="5">June</option>
            <option value="6">July</option>
            <option value="7">August</option>
            <option value="8">September</option>
            <option value="9">October</option>
            <option value="10">November</option>
            <option value="11">December</option>
          </select>

          <select id="yearSelect" onchange="changeCalendarView()" class="bg-slate-100 font-bold text-slate-800 text-sm py-1.5 px-2.5 rounded-lg border border-slate-300 outline-none focus:ring-2 focus:ring-purple-600">
            <option value="2025">2025</option>
            <option value="2026">2026</option>
            <option value="2027">2027</option>
            <option value="2028">2028</option>
          </select>
        </div>

        <!-- Jump to Today Button -->
        <button onclick="jumpToCurrentMonth()" class="text-xs font-semibold bg-purple-50 text-purple-700 px-3 py-1.5 rounded-lg hover:bg-purple-100 transition">
          Today
        </button>
      </div>

      <!-- Days of Week Header -->
      <div class="grid grid-cols-7 text-center text-xs font-bold text-slate-400 mb-2">
        <div>M</div><div>T</div><div>W</div><div>T</div><div>F</div><div>S</div><div>S</div>
      </div>

      <!-- Calendar Days Grid -->
      <div id="calendarDays" class="grid grid-cols-7 gap-1.5 text-center text-sm font-medium">
        <!-- Rendered via Javascript -->
      </div>
    </div>

    <!-- Entry Modal / Shift Selector (Simple Inline Input) -->
    <div id="shiftLoggerBox" class="bg-white p-5 rounded-2xl shadow-md border border-slate-200 hidden">
      <div class="flex justify-between items-center mb-3">
        <h3 id="selectedDateTitle" class="font-bold text-slate-800">Select Shift</h3>
        <button onclick="closeLogger()" class="text-xs text-slate-400 hover:text-slate-600">Close</button>
      </div>

      <div class="grid grid-cols-2 gap-2 mb-3">
        <button onclick="setShiftForSelectedDate('DS')" class="bg-blue-600 text-white py-2 rounded-lg text-xs font-bold hover:opacity-90">Day Shift (DS)</button>
        <button onclick="setShiftForSelectedDate('WN')" class="bg-teal-600 text-white py-2 rounded-lg text-xs font-bold hover:opacity-90">Night Shift (WN)</button>
        <button onclick="setShiftForSelectedDate('SO')" class="bg-purple-600 text-white py-2 rounded-lg text-xs font-bold hover:opacity-90">Sleepover (SO)</button>
        <button onclick="setShiftForSelectedDate('TR')" class="bg-orange-600 text-white py-2 rounded-lg text-xs font-bold hover:opacity-90">Training (TR)</button>
      </div>
      
      <button onclick="setShiftForSelectedDate(null)" class="w-full bg-slate-100 text-slate-600 py-2 rounded-lg text-xs font-semibold hover:bg-slate-200">Clear Shift</button>
    </div>

  </main>

  <script>
    const today = new Date();
    let currentDisplayMonth = today.getMonth();
    let currentDisplayYear = today.getFullYear();
    let selectedDateStr = null;

    // Load logged shifts from LocalStorage
    const STORAGE_KEY = 'orchard_roster_data';
    let loggedShifts = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {};

    function initCalendar() {
      document.getElementById('monthSelect').value = currentDisplayMonth;
      document.getElementById('yearSelect').value = currentDisplayYear;
      renderCalendar();
    }

    function changeCalendarView() {
      currentDisplayMonth = parseInt(document.getElementById('monthSelect').value);
      currentDisplayYear = parseInt(document.getElementById('yearSelect').value);
      renderCalendar();
    }

    function jumpToCurrentMonth() {
      currentDisplayMonth = today.getMonth();
      currentDisplayYear = today.getFullYear();
      document.getElementById('monthSelect').value = currentDisplayMonth;
      document.getElementById('yearSelect').value = currentDisplayYear;
      renderCalendar();
    }

    function renderCalendar() {
      const container = document.getElementById('calendarDays');
      container.innerHTML = '';

      const firstDay = new Date(currentDisplayYear, currentDisplayMonth, 1);
      const lastDay = new Date(currentDisplayYear, currentDisplayMonth + 1, 0);

      // Adjust Monday index start (0 = Mon, 6 = Sun)
      let startingDay = firstDay.getDay() - 1;
      if (startingDay === -1) startingDay = 6;

      // Blank slots before 1st of month
      for (let i = 0; i < startingDay; i++) {
        const emptyCell = document.createElement('div');
        emptyCell.className = "h-10";
        container.appendChild(emptyCell);
      }

      // Render days
      for (let day = 1; day <= lastDay.getDate(); day++) {
        const dateString = `${currentDisplayYear}-${String(currentDisplayMonth + 1).padStart(2, '0')}-${String(day).padStart(2, '0')}`;
        const dayCell = document.createElement('div');
        
        const isToday = day === today.getDate() && currentDisplayMonth === today.getMonth() && currentDisplayYear === today.getFullYear();
        
        let cellClasses = "h-10 rounded-xl flex flex-col items-center justify-center cursor-pointer border transition text-xs relative ";
        
        if (isToday) {
          cellClasses += "border-purple-600 bg-purple-50 font-bold text-purple-900 ";
        } else {
          cellClasses += "border-slate-100 bg-slate-50 text-slate-700 hover:bg-slate-100 ";
        }

        const shift = loggedShifts[dateString];
        let shiftBadge = '';
        
        if (shift === 'DS') shiftBadge = '<span class="text-[9px] font-bold text-blue-600">DS</span>';
        if (shift === 'WN') shiftBadge = '<span class="text-[9px] font-bold text-teal-600">WN</span>';
        if (shift === 'SO') shiftBadge = '<span class="text-[9px] font-bold text-purple-600">SO</span>';
        if (shift === 'TR') shiftBadge = '<span class="text-[9px] font-bold text-orange-600">TR</span>';

        dayCell.className = cellClasses;
        dayCell.innerHTML = `<span>${day}</span>${shiftBadge}`;
        dayCell.onclick = () => openLogger(dateString);

        container.appendChild(dayCell);
      }
    }

    function openLogger(dateStr) {
      selectedDateStr = dateStr;
      document.getElementById('selectedDateTitle').innerText = `Shift for ${dateStr}`;
      document.getElementById('shiftLoggerBox').classList.remove('hidden');
    }

    function closeLogger() {
      document.getElementById('shiftLoggerBox').classList.add('hidden');
    }

    function setShiftForSelectedDate(shiftType) {
      if (!selectedDateStr) return;
      
      if (shiftType) {
        loggedShifts[selectedDateStr] = shiftType;
      } else {
        delete loggedShifts[selectedDateStr];
      }

      localStorage.setItem(STORAGE_KEY, JSON.stringify(loggedShifts));
      renderCalendar();
      closeLogger();
    }

    // Startup Initialization
    initCalendar();
  </script>
</body>
</html>
