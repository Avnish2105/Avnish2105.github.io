<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Avnish Deshmukh - Robotics Enthusiast</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        h1, h2, h3 {
            margin: 0;
        }

        p {
            margin: 10px 0;
        }

        /* Flex Layout for Profile Section */
        .profile-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            margin: 20px;
        }

        .profile-container img {
            border-radius: 50%;
            width: 200px;
            height: 200px;
            margin: 10px;
            max-width: 100%;
            height: auto;
        }

        .profile-text {
            max-width: 600px;
            text-align: center;
            margin: 10px;
        }

        /* Journey Timeline */
        #journeyTimeline {
            position: relative;
            max-width: 100%;
            margin: auto;
            padding: 20px;
            border-left: 4px solid #0078D4;
            background-color: #f9f9f9;
        }

        .timeline-event {
            margin: 20px 0;
            position: relative;
            padding-left: 50px;
        }

        .timeline-event::before {
            content: attr(data-year);
            font-weight: bold;
            color: #0078D4;
            position: absolute;
            left: -70px;
            top: 0;
            font-size: 0.9em;
        }

        .timeline-event::after {
            content: '';
            position: absolute;
            left: -7px;
            top: 0;
            width: 16px;
            height: 16px;
            background-color: #0078D4;
            border-radius: 50%;
        }

        .timeline-event > div {
            background: white;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        .timeline-event h3 {
            color: #0078D4;
        }

        /* Social Links Section */
        #socialLinks {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .profile-box {
            border-radius: 12px;
            padding: 15px;
            flex: 1 1 300px;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: #f0f8ff;
            transition: transform 0.3s;
        }

        .profile-box img {
            border-radius: 50%;
            margin-bottom: 10px;
            width: 48px;
            height: 48px;
        }

        .profile-link {
            text-decoration: none;
            color: white;
            padding: 5px 8px;
            border-radius: 8px;
            margin-top: 10px;
            display: inline-block;
        }

        /* Contact Button */
        .contact-button {
            display: inline-block;
            border-radius: 12px;
            background-color: #0078D4;
            color: white;
            text-decoration: none;
            padding: 10px 20px;
            transition: background-color 0.3s, transform 0.3s;
            margin: 20px 0;
        }

        .contact-button:hover {
            background-color: #005999;
            transform: scale(1.05);
        }

        /* Back-to-Top Button */
        #backToTopBtn {
            display: none;
            position: fixed;
            bottom: 40px;
            right: 40px;
            background-color: #333;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            z-index: 1000;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .profile-container {
                flex-direction: column;
            }

            .timeline-event {
                padding-left: 20px;
            }

            .timeline-event::before {
                left: -50px;
            }

            #socialLinks {
                flex-direction: column;
            }

            .profile-box {
                margin: 10px 0;
            }

            #backToTopBtn {
                padding: 8px 16px;
                font-size: 0.9em;
                bottom: 20px;
            }
        }
    </style>
</head>
<body>

    <!-- Profile Section -->
    <div class="profile-container">
        <img src="./profile_picture.jpeg" alt="Profile Picture">
        <div class="profile-text">
            <h2>Robotics Enthusiast & Tech Innovator</h2>
            <p>
                A 🤖 robotics enthusiast, tech team member at MTT ROBOCON, and a dedicated learner passionate about 🔧 electronics, 💻 coding, and 🛠️ mechanical design. 
                I love solving complex problems and pushing the boundaries of technology. Living with ⚡ epilepsy has taught me resilience and has been an integral 
                part of my journey, shaping who I am today. Welcome to my personal website, where I share my projects, experiences, and insights from the world of 
                robotics and beyond! 🚀
            </p>
        </div>
    </div>

    <!-- Journey Timeline -->
    <div id="journeyTimeline">
        <h2 style="text-align: center; color: #0078D4;">My Journey</h2>
        
        <!-- Timeline Events -->
        <div class="timeline-event" data-year="2005">
            <h3>Born</h3>
            <p>2005</p>
        </div>
        
        <div class="timeline-event" data-year="2021">
            <h3>Completed 10th Grade</h3>
            <p>Stella Maris School</p>
        </div>

        <div class="timeline-event" data-year="2022">
            <h3>Started Diploma & Joined MIT Tech Team</h3>
            <p>Participated in DD Robocon Air 4<br>MIT World Peace University</p>
        </div>

        <div class="timeline-event" data-year="2023">
            <h3>Participated in DD Robocon Air 2</h3>
            <p>2023</p>
        </div>

        <div class="timeline-event" data-year="2024">
            <h3>Started with ROS2</h3>
            <p>Participated in DD Robocon Air 3<br>2024</p>
        </div>

        <div class="timeline-event bounce" data-year="2025" style="--color: #FF6F00;">
            <h3>Aiming for DD Robocon Air 1</h3>
            <p>2025</p>
        </div>
    </div>

    <!-- Social Links Section -->
    <div id="socialLinks">
        <!-- LinkedIn Profile Box -->
        <div class="profile-box" style="border: 2px solid #0A66C2;">
            <img src="https://img.icons8.com/color/48/000000/linkedin-circled.png" alt="LinkedIn Logo">
            <h3>Avnish Deshmukh</h3>
            <p>Robotics Enthusiast & Tech Innovator | Electronics | ROS2 | Project Management</p>
            <a href="https://www.linkedin.com/in/avnish-deshmukh" class="profile-link" style="background-color: #0A66C2;">View LinkedIn</a>
        </div>

        <!-- GitHub Profile Box -->
        <div class="profile-box" style="border: 2px solid #181717;">
            <img src="https://img.icons8.com/material-rounded/48/000000/github.png" alt="GitHub Logo">
            <h3>Avnish Deshmukh</h3>
            <p>Robotics Enthusiast & Tech Innovator | Exploring code and hardware</p>
            <a href="https://github.com/avnishd2105" class="profile-link" style="background-color: #181717;">View GitHub</a>
        </div>

        <!-- Instagram Profile Box -->
        <div class="profile-box" style="border: 2px solid #E4405F;">
            <img src="https://img.icons8.com/color/48/000000/instagram-new.png" alt="Instagram Logo">
            <h3>Avnish Deshmukh</h3>
            <p>Capturing moments & sharing my journey in tech and robotics</p>
            <a href="https://www.instagram.com/av.nish2105/" class="profile-link" style="background-color: #E4405F;">View Instagram</a>
        </div>
    </div>

    <!-- Contact Button -->
    <div style="text-align: center;">
        <a href="mailto:avnishdeshmukh2105@gmail.com" class="contact-button">Contact Me</a>
    </div>

    <!-- Back-to-Top Button -->
    <button id="backToTopBtn" onclick="scrollToTop()">Back to Top</button>

    <script>
        // Scroll-to-Top Function
        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Display back-to-top button when scrolling
        window.onscroll = function () {
            const button = document.getElementById('backToTopBtn');
            if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
                button.style.display = 'block';
            } else {
                button.style.display = 'none';
            }
        };
    </script>

</body>
</html>
