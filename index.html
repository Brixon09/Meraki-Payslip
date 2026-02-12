<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Payslip</title>

<style>
body{
    font-family: Arial, sans-serif;
    font-size: 13px;
}

.payslip{
    width:578px;
    border:1px solid #000;
    padding:7px;
}

.center{text-align:center;}

table{
    width:100%;
    border-collapse:collapse;
    margin-top:10px;
}

th,td{
    border:1px solid #000;
    padding:3.5px;
}

th{
    background:#ddd;
}

input{
    width:98%;
    border:none;
    text-align:right;
    font-size:13px;
}

input:focus{
    outline:none;
    background:#f0f0f0;
}

.bold{
    font-weight:bold;
}

.footer{
    display:flex;
    justify-content:space-between;
    margin-top:20px;
        margin-bottom:10px;
}

.signature{
    width:45%;
    text-align:center;
}

.line{
    border-top:1px solid #000;
    margin-top:40px;
    font-weight:bold;
}

/* --- Default print: Payslip Form (Landscape) --- */
/* --- Print Payslip Full Page (Portrait) --- */
@media print {
    button, .no-print { display: none; }

    /* Inputs formatting */
    input {
        border: none;
        text-align: right;
        background: transparent;
        padding: 0;
    }

    body {
        margin: 0;
        padding: 0;
    }
 th, td {
        -webkit-print-color-adjust: exact;
        print-color-adjust: exact;
    }
    /* Payslip full width */
    .payslip {
        width: 100%;          /* Full page width */
        float: none;          /* Remove float */
        box-sizing: border-box;
        page-break-inside: avoid;
        margin-top: -20px;      /* Small top margin */
        margin-bottom: 10mm;  /* Bottom margin */
        padding: 0 5mm;       /* Optional: small left-right padding */
    }

    .left-panel {
        width: 100%;
    }

    .right-panel {
        display: none;        /* Hide payslip list */
    }
    

    /* Full page Letter */
    @page {
        size: letter;         /* Portrait */
        margin: 5mm 10mm 10mm 10mm; /* Top Right Bottom Left */
    }
    
}

/* --- Print Employee Payslip List only --- */
@media print {
    body.print-list-mode {
        /* Hide everything except right panel */
        .left-panel, .payslip { display: none !important; }

        .right-panel { 
            display: block !important; 
            width: 100%; 
            border: none !important; /* REMOVE border for print */
            background: #fff !important; /* optional: make background white */
        }

        /* Hide all buttons in the table when printing */
        .right-panel button { display: none !important; }

        /* Hide Action column completely, including borders */
        #payslipTable th:last-child,
        #payslipTable td:last-child {
            display: none !important;
            border: none !important;
        }

        /* Make table fill page nicely */
        #payslipTable { 
            width: 100%; 
            border-collapse: collapse;
        }

        #payslipTable th, 
        #payslipTable td { 
            border: 1px solid #000; /* keep other borders */
        }
    }
}



/* MAIN LAYOUT */
.main-layout{
    display: flex;
    gap: 20px;
    padding: 10px;
}

/* LEFT SIDE */
.left-panel{
    flex: 2; /* mas malapad */
}

/* RIGHT SIDE */
.right-panel{
    flex: 1; /* mas makitid */
    border:1px solid #ccc;
    padding:10px;
    background:#fafafa;
    max-height:90vh;
    overflow-y:auto;
}
</style>
</head>

<body>

<div style="margin-top:10px; text-align:right;">
    <button type="button" onclick="savePayslip()">💾 Save</button>
    <button type="button" onclick="window.print()">🖨 Print</button>
</div>

<div class="main-layout">
    <!-- LEFT: Payslip Form -->
    <div class="left-panel">
<div class="payslip">

<div class="center">
    <h3>PAYSLIP</h3>
    MERAKI GARDEN<br>
    REINA MERCEDES, ISABELA
</div>

<br>

<div style="display:flex; justify-content:space-between; align-items:center; gap:20px; margin-bottom:10px;">
    
    <!-- Pay Date -->
    <div style="display:flex; align-items:center; gap:10px;">
        <label style="white-space:nowrap;">Pay Date:</label>
        <span class="no-print">
            <select id="cutoff" onchange="updatePayDate()">
                <option value="15">15th</option>
                <option value="EOM">End of Month</option>
            </select>
        </span>
        <input type="text" id="payDate" readonly style="flex:1;">
    </div>

<!-- Employee -->
<div style="display:flex; align-items:center; gap:10px;">
    <label style="white-space:nowrap;">Employee:</label>
    <input type="text" id="employee" name="employee">
</div>

</div>


<table>

<tr>
    <th colspan="2" style="background-color:#f0f0f0;">Earnings</th>
    <th colspan="2" style="background-color:#f0f0f0;">Deductions</th>
</tr>

<tr>
<td>Rate / Day</td>
<td><input id="rate" oninput="compute()"></td>

<td>STALLS</td>
<td><input class="deduct" oninput="compute()"></td>
</tr>

<tr>
<td>Total Days</td>
<td><input id="days" oninput="compute()"></td>

<td>CHARGES</td>
<td><input class="deduct" oninput="compute()"></td>
</tr>

<tr>
<td>Rate / Hour</td>
<td><input id="rateHour" readonly></td>

<td>CASH ADVANCE</td>
<td><input class="deduct" oninput="compute()"></td>
</tr>

<tr>
<td style="white-space:nowrap; background-color:white;">Total Hours (OT)</td>
<td><input id="totalHours" oninput="compute()"></td>

<td>SSS</td>
<td><input class="deduct" oninput="compute()"></td>
</tr>

<tr>
<td>Basic Pay</td>
<td><input id="basic" readonly></td>

<td>PHILHEALTH</td>
<td><input class="deduct" oninput="compute()"></td>
</tr>

<tr>
<td></td>
<td></td>

<td>PAG-IBIG</td>
<td><input class="deduct" oninput="compute()"></td>
</tr>


<tr class="bold">
<td style="white-space:nowrap; background-color:#f0f0f0;">Total Earnings</td>
<td><input id="totalEarnings" readonly></td>

<th style="white-space:nowrap; background-color:#f0f0f0;">Total Deductions</th>
<td><input id="totalDeduct" readonly></td>
</tr>

<tr class="bold">
<td colspan="3" style="text-align:right;">Net Pay</td>
<td><input id="netPay" readonly></td>
</tr>

</table>

<!-- Net Pay Footer Display -->
<div style="margin-top:20px; text-align:center;">
    <div id="netPayNumber" style="font-size:16px; font-weight:bold;">0</div>
    <div id="netPayWords" style="font-size:14px; font-style:italic;">Zero</div>
</div>


<!-- Signature Section -->
<div class="footer">

    <div class="signature">
        <div class="line">ELIZABETH COLOMA</div>
        SECRETARY
    </div>

    <div class="signature">
        <div class="line" id="signatureEmployee">EMPLOYEE</div>
        EMPLOYEE
    </div>

</div>
    </div>
</div>



<!-- RIGHT: Payslip List -->
<div class="right-panel">

    <h3>
        Employee Payslip List 
        <span id="listPayDate" style="font-size:14px; font-weight:normal; margin-left:10px;"></span>
    </h3>

    <!-- Print Button -->
    <button type="button" onclick="printPayslipList()">🖨️ Print List</button>

    <table border="1" width="100%" id="payslipTable">
        <thead>
            <tr>
                <th>#</th>
                <th>Employee</th>
                <th>Net Pay</th>
                <th>Action</th>
            </tr>
        </thead>
        <tbody>
            <!-- Auto insert dito -->
        </tbody>
    </table>

</div>
</div>


<script>

// Save all inputs to localStorage
function saveData(){
    document.querySelectorAll("input").forEach(input=>{
        localStorage.setItem(input.id || input.name, input.value);
    });
}

// Load saved data
function loadData(){
    document.querySelectorAll("input").forEach(input=>{
        let saved = localStorage.getItem(input.id || input.name);
        if(saved !== null){
            input.value = saved;
        }
    });

    compute();       // recompute earnings/deductions
    updatePayDate(); // set Pay Date after load
}

// Main compute function
function compute(){

    let rate  = Number(document.getElementById("rate").value) || 0;
    let days  = Number(document.getElementById("days").value) || 0;

    // Allow hours with H/h
    let rawHours = document.getElementById("totalHours").value;
    let hours = parseFloat(
        rawHours.replace(/[^0-9.]/g,"")
    ) || 0;

    // Rate per hour
    let rateHour = rate / 8;
    document.getElementById("rateHour").value =
        rateHour.toFixed(2);

    // Basic Pay
    let basic = rate * days;
    document.getElementById("basic").value =
        basic.toLocaleString();

    // Overtime Pay
    let overtime = rateHour * hours;

    // Total Earnings
    let totalEarnings = basic + overtime;
    document.getElementById("totalEarnings").value =
        totalEarnings.toLocaleString();

    // Deductions
    let deducts = document.querySelectorAll(".deduct");
    let totalDeduct = 0;

    deducts.forEach(d=>{
        totalDeduct += Number(d.value) || 0;
    });

    document.getElementById("totalDeduct").value =
        totalDeduct.toLocaleString();

    // Net Pay
    let net = totalEarnings - totalDeduct;
    document.getElementById("netPay").value =
        net.toLocaleString();

// -----------------------------
// Update Footer Display
// -----------------------------
const netPayNumberDiv = document.getElementById("netPayNumber");
const netPayWordsDiv  = document.getElementById("netPayWords");

if(netPayNumberDiv && netPayWordsDiv){
    netPayNumberDiv.innerText = net.toLocaleString();

    // Separate integer and decimal part
    let integerPart = Math.floor(net);
    let decimalPart = Math.round((net - integerPart) * 100); // two decimal digits

    let words = numberToWords(integerPart);
    if(decimalPart > 0){
        words += " and " + numberToWords(decimalPart) + " Centavos";
    }

    netPayWordsDiv.innerText = words;
}

    saveData(); // autosave every change
}

// -----------------------------
// Number to Words Function
// -----------------------------
function numberToWords(n){
    const ones = ["","One","Two","Three","Four","Five","Six","Seven","Eight","Nine"];
    const teens = ["Ten","Eleven","Twelve","Thirteen","Fourteen","Fifteen","Sixteen","Seventeen","Eighteen","Nineteen"];
    const tens = ["","","Twenty","Thirty","Forty","Fifty","Sixty","Seventy","Eighty","Ninety"];
    const thousand = ["","Thousand","Million","Billion"];

    if(n === 0) return "Zero";

    let word = "";
    let i = 0;

    while(n > 0){
        let chunk = n % 1000;
        if(chunk){
            word = chunkToWords(chunk) + " " + thousand[i] + " " + word;
        }
        n = Math.floor(n / 1000);
        i++;
    }

    return word.trim();
}

function chunkToWords(n){
    const ones = ["","One","Two","Three","Four","Five","Six","Seven","Eight","Nine"];
    const teens = ["Ten","Eleven","Twelve","Thirteen","Fourteen","Fifteen","Sixteen","Seventeen","Eighteen","Nineteen"];
    const tens = ["","","Twenty","Thirty","Forty","Fifty","Sixty","Seventy","Eighty","Ninety"];
    let str = "";

    if(n >= 100){
        str += ones[Math.floor(n/100)] + " Hundred ";
        n = n % 100;
    }
    if(n >= 20){
        str += tens[Math.floor(n/10)] + " ";
        n = n % 10;
    } else if(n >= 10){
        str += teens[n-10] + " ";
        n = 0;
    }
    if(n > 0){
        str += ones[n] + " ";
    }
    return str.trim();
}


// Update Pay Date based on cutoff selection
function updatePayDate(){
    const cutoff = document.getElementById("cutoff").value;
    const payInput = document.getElementById("payDate");
    const now = new Date();
    const monthNames = [
        "January","February","March","April","May","June",
        "July","August","September","October","November","December"
    ];
    const month = monthNames[now.getMonth()];
    const year = now.getFullYear();

    // Number of days in current month
    const daysInMonth = new Date(year, now.getMonth()+1, 0).getDate();

    if(cutoff === "15"){
        payInput.value = `${month} 1-15`;
    } else {
        payInput.value = `${month} 16-${daysInMonth}`;
    }

    saveData(); // save immediately
}

// --- Auto save all inputs on change ---
document.querySelectorAll("input").forEach(input=>{
    input.addEventListener("input", saveData);
});

// --- Auto update Pay Date when cutoff changes ---
document.getElementById("cutoff").addEventListener("change", updatePayDate);

// --- Sync Employee input to signature ---
const employeeInput = document.getElementById("employee");
const signatureDiv = document.getElementById("signatureEmployee");

// Update signature whenever input changes
employeeInput.addEventListener("input", function(){
    signatureDiv.innerText = employeeInput.value || "EMPLOYEE";
    localStorage.setItem("employee", employeeInput.value); // save
});

// Load saved Employee on page load
window.onload = function(){
    const savedEmployee = localStorage.getItem("employee");
    if(savedEmployee){
        employeeInput.value = savedEmployee;
        signatureDiv.innerText = savedEmployee;
    }

    loadData();       // existing function to load other inputs
    updatePayDate();  // set Pay Date
};

let payslips = JSON.parse(localStorage.getItem("payslips")) || [];

// Load list pag open
window.addEventListener("load", loadPayslipList);

function savePayslip(){

    const employee = document.getElementById("employee").value;
    const payDate  = document.getElementById("payDate").value;
    const netPay   = document.getElementById("netPay").value;

    if(!employee){
        alert("Please enter employee name");
        return;
    }

    const data = {
        id: Date.now(),
        employee,
        payDate,
        netPay
    };

    payslips.push(data);

    localStorage.setItem("payslips", JSON.stringify(payslips));

    loadPayslipList();

    alert("Payslip Saved!");
}

// Load list
function loadPayslipList() {
    const tbody = document.querySelector("#payslipTable tbody");
    tbody.innerHTML = "";

    const currentPayDate = document.getElementById("payDate").value;
    document.getElementById("listPayDate").innerText = `Pay Date: ${currentPayDate}`;

    payslips.forEach((p, i) => {
        const tr = document.createElement("tr");

        tr.innerHTML = `
            <td>${i+1}</td>
            <td>${p.employee}</td>
            <td style="text-align:right;">${p.netPay}</td>
            <td>
                <button onclick="loadPayslip(${p.id})">Edit</button>
                <button onclick="deletePayslip(${p.id})" style="color:red;">Delete</button>
            </td>
        `;

        tbody.appendChild(tr);
    });
}

// Load to form
function loadPayslip(id) {
    const p = payslips.find(x => x.id === id);
    if (!p) return;

    document.getElementById("employee").value = p.employee;
    document.getElementById("payDate").value  = p.payDate;
    document.getElementById("netPay").value   = p.netPay;

    alert("Loaded for editing");
}

// --- Delete payslip ---
function deletePayslip(id) {
    if (!confirm("Delete this payslip?")) return;

    payslips = payslips.filter(p => p.id !== id);
    localStorage.setItem("payslips", JSON.stringify(payslips));
    loadPayslipList();
}
// --- Print Employee Payslip List directly ---
function printPayslipList() {
    // Add temporary class to body to trigger CSS for list print
    document.body.classList.add("print-list-mode");

    // Trigger print
    window.print();

    // Remove class after printing
    setTimeout(() => {
        document.body.classList.remove("print-list-mode");
    }, 1000);
}

// --- Existing Save Payslip Function ---
function savePayslip() {
    const employee = document.getElementById("employee").value;
    const payDate  = document.getElementById("payDate").value;
    const netPay   = document.getElementById("netPay").value;

    if (!employee) {
        alert("Please enter employee name");
        return;
    }

    const data = {
        id: Date.now(),
        employee,
        payDate,
        netPay
    };

    payslips.push(data);
    localStorage.setItem("payslips", JSON.stringify(payslips));

    loadPayslipList();
    alert("Payslip Saved!");
}

let payslipEntries = []; // global array para sa lahat ng payslips


//2️⃣ Render Function
function renderPayslipList(){
    const tbody = document.querySelector("#payslipTable tbody");
    tbody.innerHTML = "";

    payslipEntries.forEach((entry, index) => {
        const tr = document.createElement("tr");

        tr.innerHTML = `
            <td>${index+1}</td>
            <td>${entry.employee}</td>
            <td>${entry.netPay.toLocaleString()}</td>
            <td>
                <button onclick="editPayslip(${entry.id})">Edit</button>
                <button onclick="deletePayslip(${entry.id})">Delete</button>
            </td>
        `;

        tbody.appendChild(tr);
    });
}
//3️⃣ Edit at Delete
function editPayslip(id){
    const entry = payslipEntries.find(e => e.id === id);
    if(!entry) return;

    // Fill form
    document.getElementById("employee").value = entry.employee;
    document.getElementById("payDate").value = entry.payDate;
    document.getElementById("rate").value = entry.rate;
    document.getElementById("days").value = entry.days;
    document.getElementById("totalHours").value = entry.totalHours;

    const deducts = document.querySelectorAll(".deduct");
    deducts[0].value = entry.stalls;
    deducts[1].value = entry.charges;
    deducts[2].value = entry.cashAdvance;
    deducts[3].value = entry.sss;
    deducts[4].value = entry.philhealth;
    deducts[5].value = entry.pagibig;

    // Recompute totals
    compute();

    window.scrollTo({ top: 0, behavior: 'smooth' });
}


</script>



</body>
</html>
