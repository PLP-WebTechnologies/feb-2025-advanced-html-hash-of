# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced HTML5 Elements and Forms</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 10px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 5px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
            margin-top: 5px;
        }
        input[type="radio"], input[type="checkbox"] {
            width: auto;
            margin-right: 10px;
        }
        .checkbox-group, .radio-group {
            margin-top: 5px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Advanced HTML5 Elements Demonstration</h1>
    </header>

   <section>
        <h2>Ordered List with Roman Numerals</h2>
        <!-- Ordered list with roman numerals -->
        <ol type="i">
            <li>Introduction to HTML5</li>
            <li>Semantic Elements</li>
            <li>Forms and Validation</li>
            <li>Multimedia Elements</li>
            <li>Responsive Design</li>
        </ol>
    </section>

   <section>
        <h2>External Image</h2>
        <!-- External image from Pexels -->
        <img src="https://images.pexels.com/photos/270348/pexels-photo-270348.jpeg" 
             alt="Coding on computer screen" 
             width="600">
    </section>

   <section>
        <h2>Contact Table</h2>
        <!-- Table with 5 contacts -->
        <table>
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John gathegee</td>
                    <td>123 Main St, City</td>
                    <td>555-1264</td>
                    <td>john@yahoo.com</td>
                </tr>
                <tr>
                    <td>Jane whosh</td>
                    <td>456 Oak Ave, Town</td>
                    <td>555-5678</td>
                    <td>jane@gmail.com</td>
                </tr>
                <tr>
                    <td>Michael son</td>
                    <td>789 Pine Rd, Village</td>
                    <td>555-9012</td>
                    <td>michael@yahoo.com</td>
                </tr>
                <tr>
                    <td>Sarah liams</td>
                    <td>321 Cedar Ln, Borough</td>
                    <td>555-3456</td>
                    <td>sarah@gmail.com</td>
                </tr>
                <tr>
                    <td>Robert Bangoi</td>
                    <td>654 Birch Dr, County</td>
                    <td>555-7890</td>
                    <td>robert@yahoo.com</td>
                </tr>
            </tbody>
        </table>
    </section>

   <section>
        <h2>Registration Form</h2>
        <!-- Registration form with required fields and validation -->
        <form id="registrationForm" action="#" method="post">
            <!-- Name field -->
            <div class="form-group">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
            </div>
 <!-- Email field -->
            <div class="form-group">
                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>
            </div>
 <!-- Password field -->
            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" placeholder="Choose a password" 
                       minlength="8" required>
            </div>
 <!-- Date field -->
            <div class="form-group">
                <label for="birthdate">Date of Birth:</label>
                <input type="date" id="birthdate" name="birthdate" required>
            </div>

  <!-- Dropdown/Select field -->
   <div class="form-group">
                <label for="country">Country:</label>
                <select id="country" name="country" required>
                    <option value="">--Select a country--</option>
                    <option value="us">United States</option>
                    <option value="ca">Canada</option>
                    <option value="uk">United Kingdom</option>
                    <option value="au">Australia</option>
                    <option value="other">Other</option>
                </select>
            </div>

   <!-- Radio buttons -->
  <div class="form-group">
                <label>Gender:</label>
                <div class="radio-group">
                    <input type="radio" id="male" name="gender" value="male" required>
                    <label for="male">Male</label>
                    
   <input type="radio" id="female" name="gender" value="female">
                    <label for="female">Female</label>
                    
   <input type="radio" id="other" name="gender" value="other">
                    <label for="other">Other</label>
                </div>
            </div>

  <!-- Checkboxes -->
 <div class="form-group">
                <label>Interests (select all that apply):</label>
                <div class="checkbox-group">
                    <input type="checkbox" id="web" name="interests" value="web">
                    <label for="web">Web Development</label><br>
                    
  <input type="checkbox" id="mobile" name="interests" value="mobile">
          <label for="mobile">Mobile Development</label><br>
                    
   <input type="checkbox" id="data" name="interests" value="data">
                    <label for="data">Data Science</label><br>
                    
   <input type="checkbox" id="design" name="interests" value="design">
                    <label for="design">UI/UX Design</label>
                </div>
            </div>

  <!-- Submit button -->
  <div class="form-group">
                <button type="submit">Register</button>
            </div>
        </form>
    </section>

 <!-- Multimedia elements -->
  <section>
        <h2>Multimedia Elements</h2>
        
   <h3>Audio Example</h3>
        <!-- Audio element -->
        <audio controls>
            <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>

   <h3>Video Example</h3>
        <!-- Video element -->
        <video width="400" controls>
            <source src="https://sample-videos.com/video123/mp4/240/big_buck_bunny_240p_1mb.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </section>

   <footer>
        <p>&copy; 2025 Advanced HTML5 Elements Demo</p>
    </footer>
</body>
</html>
