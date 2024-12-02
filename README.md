### Assignment: Building a Multimedia Webpage and a Registration Form  

#### Objective: 
The goal of this assignment is to create a multimedia-rich webpage featuring audio and video elements and design a simple registration form with built-in HTML validation.  

---

### Part 1: Multimedia Webpage 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multimedia Webpage</title>
</head>
<body>
    <h1>Multimedia Webpage</h1>
    
    <h2>Audio Player</h2>
    <audio controls>
        <source src="your-audio-file.mp3" type="audio/mp3">
        <source src="your-audio-file.ogg" type="audio/ogg">
        Your browser does not support the audio element.
    </audio>

    <h2>Video Player</h2>
    <video width="600" controls poster="your-video-poster.jpg">
        <source src="your-video-file.mp4" type="video/mp4">
        <source src="your-video-file.webm" type="video/webm">
        Your browser does not support the video element.
    </video>

</body>
</html>


### **Part 2: Registration Form **  
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Form</title>
</head>
<body>
    <h1>User Registration Form</h1>

    <form action="submit-form.php" method="post">
        <label for="full-name">Full Name:</label>
        <input type="text" id="full-name" name="full-name" required maxlength="100"><br><br>

        <label for="email">Email Address:</label>
        <input type="email" id="email" name="email" required><br><br>

        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required minlength="8"><br><br>

        <label for="age">Age:</label>
        <input type="number" id="age" name="age" required min="18"><br><br>

        <label>Gender:</label>
        <input type="radio" id="male" name="gender" value="male" required>
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female" required>
        <label for="female">Female</label>
        <input type="radio" id="other" name="gender" value="other" required>
        <label for="other">Other</label><br><br>

        <label for="terms">I agree to the Terms and Conditions:</label>
        <input type="checkbox" id="terms" name="terms" required><br><br>

        <button type="submit">Register</button>
    </form>

</body>
</html>
