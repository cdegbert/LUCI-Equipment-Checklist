<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LUCI Office Equipment Checklist</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f5f5f5;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        h1 {
            color: #2c3e50;
            text-align: center;
            margin-bottom: 30px;
            border-bottom: 3px solid #3498db;
            padding-bottom: 10px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
            vertical-align: top;
        }
        th {
            background-color: #3498db;
            color: white;
            font-weight: bold;
            position: sticky;
            top: 0;
        }
        tr:nth-child(even) {
            background-color: #f9f9f9;
        }
        tr:hover {
            background-color: #e8f4f8;
        }
        .checkbox {
            width: 18px;
            height: 18px;
            margin: 0;
            cursor: pointer;
            transform: scale(1.2);
        }
        .received {
            background-color: #d4edda;
        }
        .in-stock {
            background-color: #fff3cd;
        }
        .shipped {
            background-color: #f8d7da;
        }
        .waiting {
            background-color: #e2e3e5;
        }
        .status {
            font-weight: bold;
            padding: 4px 8px;
            border-radius: 4px;
            font-size: 0.85em;
        }
        .status.in-stock {
            background-color: #ffeaa7;
            color: #2d3436;
        }
        .status.shipped {
            background-color: #fab1a0;
            color: #2d3436;
        }
        .status.waiting {
            background-color: #a29bfe;
            color: white;
        }
        .status.pickup {
            background-color: #fd79a8;
            color: white;
        }
        .quantity {
            font-weight: bold;
            color: #2980b9;
        }
        .notes {
            font-style: italic;
            color: #666;
            font-size: 0.9em;
        }
        .summary {
            margin-top: 30px;
            padding: 20px;
            background-color: #ecf0f1;
            border-radius: 5px;
        }
        .progress {
            margin-top: 10px;
            height: 20px;
            background-color: #ddd;
            border-radius: 10px;
            overflow: hidden;
        }
        .progress-bar {
            height: 100%;
            background-color: #27ae60;
            width: 0%;
            transition: width 0.3s ease;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>LUCI Office Equipment Arrival Checklist</h1>
        
        <table id="checklistTable">
            <thead>
                <tr>
                    <th>✓</th>
                    <th>Qty</th>
                    <th>Item</th>
                    <th>Status</th>
                    <th>Shipping Method</th>
                    <th>Arrival Date</th>
                    <th>Notes</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>COM3000</td>
                    <td><span class="status pickup">To Pickup</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI to pickup</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">5</td>
                    <td>iPads with rugged case</td>
                    <td><span class="status shipped">Arriving</span></td>
                    <td>-</td>
                    <td>9/2</td>
                    <td class="notes">Arriving 9/2</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>NX5</td>
                    <td><span class="status in-stock">In Stock</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI has in stock</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>PD-815SC-PBSH</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>R&L</td>
                    <td>8/19</td>
                    <td class="notes">Shipped via R&L arrived 8/19</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>PDX-920R</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>R&L</td>
                    <td>8/19</td>
                    <td class="notes">Shipped via R&L arrived 8/19</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">70</td>
                    <td>STB-6500</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/15</td>
                    <td class="notes">Shipped via FedEx arrived 8/15</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>PT-FRZ60WU7</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via FedEx arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>VCMU</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via FedEx arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>ACCXWPHDMOBKT</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/13</td>
                    <td class="notes">Shipped via FedEx arrived 8/13</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">3</td>
                    <td>NUC Server</td>
                    <td><span class="status shipped">Arrived</span></td>
                    <td>-</td>
                    <td>8/13</td>
                    <td class="notes">Arrived 8/13</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>H2 Chassis</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/26</td>
                    <td class="notes">Shipped via FedEx arrived 8/26</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>H_1xHDMI2.0 Input Card</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/26</td>
                    <td class="notes">Shipped via FedEx arrived 8/26</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>H_16xRJ45+2xFiber Sending Card</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/26</td>
                    <td class="notes">Shipped via FedEx arrived 8/26</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>NG-2100</td>
                    <td><span class="status in-stock">In Stock</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI has in stock</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>CORE 24f</td>
                    <td><span class="status shipped">Shipping</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">Shipping 8/28</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>SLDAN-32-P</td>
                    <td><span class="status shipped">Emailed</span></td>
                    <td>Email</td>
                    <td>-</td>
                    <td class="notes">Emailed to LUCI 8/13</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>CX-Q 8K8</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/22</td>
                    <td class="notes">Shipped via FedEx arrived 8/22</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>QIO-ML2x2</td>
                    <td><span class="status in-stock">In Stock</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI has in stock</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>QIO-RMK</td>
                    <td><span class="status in-stock">In Stock</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI has in stock</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">4</td>
                    <td>TX-J2</td>
                    <td><span class="status in-stock">In Stock</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI has in stock</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>ULXD4Q-H50</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via UPS arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">8</td>
                    <td>ULXD2-BETA58-H50</td>
                    <td><span class="status in-stock">In Stock</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI has in stock</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>ULXD1-H50</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via UPS arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">8</td>
                    <td>SB900B</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via UPS arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">4</td>
                    <td>SBC200-US</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via UPS arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">6</td>
                    <td>UA864US</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18 & 8/22</td>
                    <td class="notes">4 of 6 shipped via UPS arrived 8/18. 2 of 6 shipped via UPS arrived 8/22</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>Omega-8 Multizone</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via FedEx arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>X32 Rack</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via UPS arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>Xdante</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>UPS</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via UPS arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">-</td>
                    <td>Stage Cables</td>
                    <td><span class="status waiting">Waiting</span></td>
                    <td>-</td>
                    <td>TBD</td>
                    <td class="notes">Waiting on ETA</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>SR-24-32</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>R&L</td>
                    <td>8/19</td>
                    <td class="notes">Shipped via R&L arrived 8/19</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">2</td>
                    <td>TD-3</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>R&L</td>
                    <td>8/19</td>
                    <td class="notes">Shipped via R&L arrived 8/19</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>PD-1820R-RN</td>
                    <td><span class="status shipped">Shipped</span></td>
                    <td>FedEx</td>
                    <td>8/18</td>
                    <td class="notes">Shipped via FedEx arrived 8/18</td>
                </tr>
                <tr>
                    <td><input type="checkbox" class="checkbox" onchange="updateProgress()"></td>
                    <td class="quantity">1</td>
                    <td>Patch cables</td>
                    <td><span class="status pickup">To Bring</span></td>
                    <td>-</td>
                    <td>-</td>
                    <td class="notes">LUCI to bring to jobsite</td>
                </tr>
            </tbody>
        </table>

        <div class="summary">
            <h3>Progress Summary</h3>
            <p>Items checked: <span id="checkedCount">0</span> of <span id="totalCount">33</span></p>
            <div class="progress">
                <div class="progress-bar" id="progressBar"></div>
            </div>
            <p id="percentageText">0% Complete</p>
        </div>
    </div>

    <script>
        function updateProgress() {
            const checkboxes = document.querySelectorAll('.checkbox');
            const totalItems = checkboxes.length;
            const checkedItems = document.querySelectorAll('.checkbox:checked').length;
            const percentage = Math.round((checkedItems / totalItems) * 100);
            
            document.getElementById('checkedCount').textContent = checkedItems;
            document.getElementById('totalCount').textContent = totalItems;
            document.getElementById('progressBar').style.width = percentage + '%';
            document.getElementById('percentageText').textContent = percentage + '% Complete';
            
            // Add visual feedback for checked rows
            checkboxes.forEach((checkbox, index) => {
                const row = checkbox.closest('tr');
                if (checkbox.checked) {
                    row.style.backgroundColor = '#d4edda';
                    row.style.opacity = '0.7';
                } else {
                    row.style.backgroundColor = '';
                    row.style.opacity = '1';
                }
            });
        }
        
        // Initialize progress on page load
        updateProgress();
    </script>
</body>
</html>
