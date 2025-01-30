<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Buttons</title>
  <style>
    /* General styling */
    body {
      overflow: hidden;
      margin: 0;
      font-family: 'Arial', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: linear-gradient(45deg, #fdc830, #f37335, #833ab4, #fd1d1d, #fcb045);
      background-size: 300% 300%;
      animation: instagramBackground 6s infinite alternate;
    }

    /* Background animation */
    @keyframes instagramBackground {
      0% {
        background-position: 0% 50%;
      }
      50% {
        background-position: 50% 100%;
      }
      100% {
        background-position: 100% 50%;
      }
    }

    /* Message styling */
    .message {
      position: absolute;
      top: 10%;
      text-align: center;
      font-size: 32px;
      font-weight: bold;
      color: white;
      text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.6);
      animation: fadeIn 2s ease;
    }

    /* Button styling */
    button {
      position: absolute;
      padding: 15px 30px;
      font-size: 18px;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      transition: all 0.5s ease;
      box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.2);
    }

    button:hover {
      transform: scale(1.1);
      box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.4);
    }

    #animatedButton {
      background: linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
      color: white;
    }

    #noButton {
      background: linear-gradient(to right, #833ab4, #fd1d1d, #fcb045);
      color: white;
    }

    /* Notification styling */
    .notification {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      padding: 20px;
      font-size: 24px;
      font-weight: bold;
      color: white;
      background: rgba(0, 0, 0, 0.8);
      border-radius: 10px;
      box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.5);
      display: none;
      text-align: center;
    }

    /* Fade-in effect */
    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }
  </style>
</head>
<body>
  <div class="message">DO YOU LOVE ME?</div>

  <button id="animatedButton" onclick="handleYesClick()">Yes</button>
  <button id="noButton" onclick="moveNoButton()">No</button>

  <div class="notification" id="notification">I LOVE YOU TOO! ❤️</div>

  <script>
    // Function to move the "No" button randomly on click
    function moveNoButton() {
      const noButton = document.getElementById('noButton');

      // Generate random positions within the window bounds
      const newX = Math.random() * (window.innerWidth - noButton.offsetWidth);
      const newY = Math.random() * (window.innerHeight - noButton.offsetHeight);

      // Update button position with a smooth transition
      noButton.style.position = 'absolute';
      noButton.style.left = `${newX}px`;
      noButton.style.top = `${newY}px`;
    }

    // Function to handle "Yes" button click
    function handleYesClick() {
      // Show the notification with a fade-in effect
      const notification = document.getElementById('notification');
      notification.style.display = 'block';
      notification.style.animation = 'fadeIn 1s ease';

      // Redirect to Instagram reel after 3 seconds
      setTimeout(() => {
        window.location.href = "https://www.instagram.com/reel/DD4-X7HzSZZ/?utm_source=ig_web_copy_link";
      }, 3000);
    }

    // Set initial position of the "No" button
    window.onload = () => {
      const noButton = document.getElementById('noButton');
      noButton.style.left = "50%";
      noButton.style.top = "50%";
      noButton.style.transform = "translate(-50%, -50%)";
    };
  </script>
</body>
</html>
