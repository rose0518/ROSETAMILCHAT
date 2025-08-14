<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Rose ChatApp 🚀</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Screen 1: Welcome / Login / Register -->
  <div id="screen1" class="screen active">
    <h1>Welcome to Rose ChatApp</h1>
    <button id="btnLogin">Login</button>
    <button id="btnRegister">Register</button>
  </div>

  <!-- Login Modal -->
  <div id="loginModal" class="modal">
    <div class="modal-content">
      <h2>Login</h2>
      <input type="text" id="loginUser" placeholder="Username">
      <input type="password" id="loginPass" placeholder="Password">
      <button id="doLogin">Login</button>
      <button class="close" data-target="loginModal">Close</button>
    </div>
  </div>

  <!-- Register Modal -->
  <div id="registerModal" class="modal">
    <div class="modal-content">
      <h2>Register</h2>
      <input type="text" id="regUser" placeholder="Username">
      <input type="password" id="regPass" placeholder="Password">
      <input type="email" id="regEmail" placeholder="Email">
      <select id="regGender">
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
      </select>
      <input type="number" id="regAge" placeholder="Age">
      <button id="doRegister">Register</button>
      <button class="close" data-target="registerModal">Close</button>
    </div>
  </div>

  <!-- Screen 3: Home Screen -->
  <div id="homeScreen" class="screen">
    <header>
      <h1>Rose ChatApp</h1>
      <button id="btnProfile">Profile</button>
    </header>
    <div class="rooms">
      <button class="room-btn" data-room="main">Main Room</button>
      <button class="room-btn" data-room="game">Game Room</button>
      <button class="room-btn" data-room="event">Event Room</button>
      <button class="room-btn" data-room="quiz">Quiz Room</button>
      <button class="room-btn" data-room="singing">Singing Room</button>
      <button class="room-btn" data-room="staff">Staff Meeting Room</button>
    </div>
    <div id="chatArea"></div>
    <div id="chatInput">
      <input type="text" id="messageInput" placeholder="Type a message...">
      <button id="btnEmoji">😊</button>
      <button id="btnSend">Send</button>
      <button id="btnRefresh">🔄</button>
    </div>
  </div>

  <!-- Profile Modal -->
  <div id="profileModal" class="modal">
    <div class="modal-content">
      <h2>Your Profile</h2>
      <div id="profileDisplay">
        <img id="profileDp" src="dp-placeholder.jpg" alt="Profile DP">
        <h3 id="profileName">Name</h3>
        <p id="profileMood">Mood...</p>
        <p id="profileAbout">About me...</p>
        <button id="btnEditProfile">Edit Profile</button>
      </div>
      <div id="profileEdit" class="hidden">
        <input type="text" id="editName">
        <input type="text" id="editMood">
        <textarea id="editAbout"></textarea>
        <button id="saveProfile">Save</button>
      </div>
      <button class="close" data-target="profileModal">Close</button>
    </div>
  </div>

  <!-- Quiz Bot Prompt -->
  <div id="quizBotModal" class="modal">
    <div class="modal-content">
      <h2>Quiz Bot</h2>
      <div id="quizQuestion">Q. ...</div>
      <input type="text" id="quizAnswer" placeholder="Your answer">
      <button id="submitQuiz">Submit</button>
      <button class="close" data-target="quizBotModal">Close</button>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
