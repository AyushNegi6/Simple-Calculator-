# Simple-Calculator-
Calculator Using Java-Script.
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
</head>

<body>
    <!-- step =  any is used so that we can store decimal value also  -->
    <input type="number" name="number" id="first" step="any">
    <select  id="operator">
        <option value="+">+</option>
        <option value="-">-</option>
        <option value="*">x</option>
        <option value="/">/</option>
    </select>
    <input type="number" name="number" id="second" step="any">
    <br />
    <button onclick="calculate()">Result</button>
    <input type="" name="" id="result" readonly="">
    <!-- read only is for only reading purpose we cant chnage it -->

    <!-- javascript -->
    <script>
        function calculate() {
            var firstnumber = document.getElementById('first').value;
            var secondnumber = document.getElementById('second').value;
            var operator = document.getElementById('operator').value;
            if (operator == '+')
            {
                var result = parseInt(firstnumber) + parseInt(secondnumber); //parseInt is used to convert string into integer 
            }
            if (operator == '-')
            {
                var result = parseInt(firstnumber) - parseInt(secondnumber);
            }
            if (operator == '*')
            {
                var result = parseInt(firstnumber) * parseInt(secondnumber);
            }
            if (operator == '/')
            {
                var result = parseInt(firstnumber) / parseInt(secondnumber);
            }
            document.getElementById('result').value = result;
            
        }
    </script>


</body>

</html>
