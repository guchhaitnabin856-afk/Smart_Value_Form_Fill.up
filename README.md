<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SmartValue Admission Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 0;
            padding: 20px;
        }
        .form-container {
            max-width: 600px;
            margin: auto;
            background: #fff;
            padding: 20px 30px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        h2 {
            text-align: center;
            color: #333;
        }
        fieldset {
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 20px;
            padding: 15px;
        }
        legend {
            font-weight: bold;
            color: #555;
            padding: 0 5px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
            color: #333;
        }
        input[type="text"],
        input[type="email"],
        input[type="tel"],
        input[type="date"],
        select,
        textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box; 
        }
        .radio-group label {
            display: inline-block;
            font-weight: normal;
            margin-right: 15px;
        }
        button {
            width: 100%;
            padding: 12px;
            background-color: #0056b3;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
        }
        button:hover {
            background-color: #004494;
        }
    </style>
</head>
<body>

<div class="form-container">
    <h2>SmartValue Course Admission Form</h2>
    <form action="/submit-admission" method="POST">
        
   <fieldset>
            <legend>Personal Information</legend>
            <div class="form-group">
                <label for="firstName">First Name</label>
                <input type="text" id="firstName" name="firstName" required placeholder="Enter your first name">
            </div>
            
  <div class="form-group">
                <label for="lastName">Last Name</label>
                <input type="text" id="lastName" name="lastName" required placeholder="Enter your last name">
            </div>

   <div class="form-group">
                <label for="dob">Date of Birth</label>
                <input type="date" id="dob" name="dob" required>
            </div>

  <div class="form-group radio-group">
                <label>Gender:</label>
                <input type="radio" id="male" name="gender" value="Male" required>
                <label for="male">Male</label>
                
   <input type="radio" id="female" name="gender" value="Female">
                <label for="female">Female</label>
                    <input type="radio" id="other" name="gender" value="Other">
                <label for="other">Other</label>
            </div>
        </fieldset>

  <fieldset>
            <legend>Contact Details</legend>
            <div class="form-group">
                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" required placeholder="example@email.com">
            </div>

   <div class="form-group">
                <label for="phone">Phone Number</label>
                <input type="tel" id="phone" name="phone" required placeholder="123-456-7890">
            </div>

  <div class="form-group">
                <label for="address">Home Address</label>
                <textarea id="address" name="address" rows="3" required placeholder="Enter your full address"></textarea>
            </div>
        </fieldset>

  <fieldset>
            <legend>Academic Information</legend>
            <div class="form-group">
                <label for="prevSchool">Previous School/College Name</label>
                <input type="text" id="prevSchool" name="prevSchool" required placeholder="Name of institution">
            </div>

   <div class="form-group">
                <label for="course">SmartValue Course Applying For</label>
                <select id="course" name="course" required>
                    <option value="" disabled selected>Select a SmartValue Course</option>
                    <option value="it_smart_plus">IT Smart Plus</option>
                    <option value="smart_commerce_plus">Smart Commerce Plus</option>
                    <option value="smart_pro_ai">SMART ProAI</option>
                    <option value="smart_webtech">Smart Webtech Online Course</option>
                    <option value="digital_rise">Digital Rise</option>
                </select>
            </div>
        </fieldset>

   <button type="submit">Submit Application</button>

  </form>
</div>

</body>
</html>
