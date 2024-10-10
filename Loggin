<!doctype html>
<html lang="en"> 
 <head> 
  <meta charset="UTF-8"> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Student Card QR Code Generator</title> 
  <script src="https://cdn.jsdelivr.net/npm/qrious/dist/qrious.min.js"></script> 
  <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 0;
            background-color: blue;
        }
        .container {
            width: 300px;
            margin: 0 auto;
            text-align: center;
            background-color: orange;
            padding: 10px;
        }
        input {
            margin-bottom: 10px;
            padding: 5px;
            width: 95%;
            border-radius: none;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
        }
        canvas {
            margin-top: 20px;
        }
    </style> 
 </head> 
 <body> 
  <div class="container"> 
   <h1>Student Card QR Generator</h1> 
   <input type="text" id="name" placeholder="Enter Your Name" required> 
   <br> 
   <input type="text" id="idNumber" placeholder="Enter Your ID Number" required> 
   <br> 
   <input type="number" id="studentNumber" placeholder="Enter Your Student Number" required> 
   <br> 
   <input type="text" placeholder="Enter your campus name" id="campus"> 
   <br> <button onclick="generateQRCode()">Generate QR Code</button> 
   <canvas id="qrCodeCanvas"></canvas> 
  </div> 
  <script>
        function generateQRCode() {
            const name = document.getElementById("name").value;
            const idNumber = document.getElementById("idNumber").value;
            const studentNumber = document.getElementById("studentNumber").value;
            const campus = document.getElementById("campus").value;
            
            if (!name || !idNumber || !studentNumber || !campus) {
                alert("Please fill in all fields");
                return;
            }

            const studentCardURL = https://example.com/student-card?name=${encodeURIComponent(name)}&campus=${encodeURIComponent(campus)}&id=${encodeURIComponent(idNumber)}&student=${encodeURIComponent(studentNumber)};

            const qr = new QRious({
                element: document.getElementById("qrCodeCanvas"),
                size: 200,
                value: studentCardURL
            });
            qr.innerHTML = "";
        }
    </script> 
 </body>
</html>
