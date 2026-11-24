<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Escape Room Magicus</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; margin-top: 100px; }
        input, button { padding: 10px; font-size: 16px; margin: 5px; }
        .error { color: red; margin-top: 10px; display: none; }
    </style>
</head>
<body>

    <h2>metti il codice:</h2>
    <h1>VHFUHW123<h1>
	
    <!-- Input box and Button -->
    <input type="text" id="passcode" placeholder="Enter code here...">
    <button onclick="checkCode()">Submit</button>
    
    <!-- Error message placeholder -->
    <div id="errorMessage" class="error">codice incoreto (sug cifr ces)</div>

    <script>
        function checkCode() {
            // 1. Get the value the user typed in
            const userInput = document.getElementById("passcode").value;
            
            // 2. Define the correct code and target page
            const correctCode = "SECRET123"; 
            const targetPage = "file:///C:/Users/26-info-05/Downloads/61-RsL8RAnL._AC_UL450_SY450_QL70_.jpg"; // Change to your destination URL or file (e.g., "success.html")

            // 3. Check if it matches
            if (userInput === correctCode) {
                window.location.href = targetPage; // Redirects the page
            } else {
                document.getElementById("errorMessage").style.display = "block"; // Shows error
            }
        }
    </script>

</body>
</html>
