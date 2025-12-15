# Personal-Profile-
Beginner developer. Learning. Building. Growing.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aysha Yimam | Personal Profile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: #333;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .profile-card {
            background: white;
            border-radius: 20px;
            width: 100%;
            max-width: 500px;
            padding: 40px 30px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .profile-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 8px;
            background: linear-gradient(90deg, #ff7e5f, #feb47b);
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid #f0f0f0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            margin: 0 auto 20px;
        }
        
        h1 {
            color: #2c3e50;
            font-size: 2.2rem;
            margin-bottom: 8px;
        }
        
        .title {
            color: #ff7e5f;
            font-weight: 600;
            margin-bottom: 25px;
            font-size: 1.1rem;
        }
        
        .bio {
            color: #555;
            line-height: 1.6;
            margin-bottom: 30px;
            font-size: 1rem;
        }
        
        .form-container {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 15px;
            margin-top: 20px;
        }
        
        h2 {
            color: #2c3e50;
            margin-bottom: 20px;
            font-size: 1.5rem;
        }
        
        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            color: #555;
            font-weight: 500;
        }
        
        input, textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
            transition: all 0.3s;
        }
        
        input:focus, textarea:focus {
            border-color: #ff7e5f;
            outline: none;
            box-shadow: 0 0 0 2px rgba(255, 126, 95, 0.2);
        }
        
        textarea {
            min-height: 100px;
            resize: vertical;
        }
        
        .submit-btn {
            background: linear-gradient(to right, #ff7e5f, #feb47b);
            color: white;
            border: none;
            padding: 14px 30px;
            font-size: 1rem;
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 600;
            width: 100%;
            margin-top: 10px;
        }
        
        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(255, 126, 95, 0.3);
        }
        
        .success-message {
            background-color: #d4edda;
            color: #155724;
            padding: 12px;
            border-radius: 8px;
            margin-top: 15px;
            display: none;
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 25px;
        }
        
        .social-icons a {
            width: 40px;
            height: 40px;
            background: #f0f0f0;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #555;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .social-icons a:hover {
            background: #ff7e5f;
            color: white;
            transform: translateY(-3px);
        }
        
        .credit {
            margin-top: 20px;
            font-size: 0.9rem;
            color: #888;
        }
    </style>
</head>
<body>
    <div class="profile-card">
        <!-- Replace the src with your actual image file path -->
        <img src="https://i.supaimg.com/91904e49-dd7f-4c12-849c-b291d6448e73.jpg" alt="Aysha Yimam" class="profile-img">
        
        <h1>Aysha Yimam</h1>
        <p class="title">Electrical Engineering and Computing Student</p>
        
        <p class="bio">
            I am a dedicated student with a passion for web development. I am currently focusing on mastering many skills and am always looking for new challenges. When I'm not coding, I enjoy learning new things and skills.
        </p>
        
        <div class="form-container">
            <h2>Get In Touch</h2>
            <form id="contactForm">
                <div class="form-group">
                    <label for="name">Your Name</label>
                    <input type="text" id="name" placeholder="Enter your name" required>
                </div>
                
                <div class="form-group">
                    <label for="email">Your Email</label>
                    <input type="email" id="email" placeholder="Enter your email" required>
                </div>
                
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea id="message" placeholder="Your message here..." required></textarea>
                </div>
                
                <button type="submit" class="submit-btn">
                    <i class="fas fa-paper-plane"></i> Send Message
                </button>
                
                <div class="success-message" id="successMessage">
                    <i class="fas fa-check-circle"></i> Message sent successfully!
                </div>
            </form>
        </div>
        
        <div class="social-icons">
            <a href="#" title="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
            <a href="#" title="Instagram"><i class="fab fa-instagram"></i></a>
            <a href="#" title="GitHub"><i class="fab fa-github"></i></a>
            <a href="#" title="Email"><i class="fas fa-envelope"></i></a>
        </div>
        
        <p class="credit">Part of Mudassir's Collection</p>
    </div>

    <script>
        document.getElementById('contactForm').addEventListener('submit', function(event) {
            event.preventDefault();
            
            const name = document.getElementById('name').value.trim();
            const email = document.getElementById('email').value.trim();
            const message = document.getElementById('message').value.trim();
            
            if(name && email && message) {
                // Show success message
                document.getElementById('successMessage').style.display = 'block';
                
                // Reset form after 2 seconds
                setTimeout(() => {
                    document.getElementById('contactForm').reset();
                    document.getElementById('successMessage').style.display = 'none';
                    
                    // Simple alert confirmation
                    alert(`Thanks, ${name}! I'll respond soon.`);
                }, 2000);
            } else {
                alert('Please fill in all fields.');
            }
        });
    </script>
</body>
</html>
