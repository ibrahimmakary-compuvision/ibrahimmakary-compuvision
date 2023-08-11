<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title> Ibrahim Makary - Senior Flutter Developer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      background-color: #f5f5f5;
    }
    .header {
      text-align: center;
      margin-bottom: 20px;
    }
    .avatar {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
    }
    .bio {
      text-align: center;
      margin-bottom: 20px;
    }
    .badge {
      display: inline-block;
      padding: 5px 10px;
      margin: 0 5px;
      background-color: #007bff;
      color: #fff;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <div class="header">
    <img class="avatar" src="https://avatars.githubusercontent.com/u/ibrahimmakary-compuvision" alt="Profile Avatar">
    <h1>[Your Name]</h1>
    <p>Senior Flutter Developer @ Compu-Vision</p>
  </div>

  <div class="bio">
    <p>I'm a passionate Flutter developer with 4 years of experience, dedicated to crafting beautiful and efficient mobile applications. Let's turn ideas into reality!</p>
  </div>

  <div class="badges">
    <a class="badge" href="https://www.linkedin.com/in/yourusername/">LinkedIn</a>
    <a class="badge" href="https://twitter.com/yourusername">Twitter</a>
    <a class="badge" href="mailto:your.email@example.com">Email</a>
  </div>

  <!-- Display GitHub Stats using GitHub API and JavaScript -->
  <div class="github-stats">
    <p>Loading GitHub Stats...</p>
    <script>
      fetch('https://api.github.com/users/ibrahimmakary-compuvision')
        .then(response => response.json())
        .then(data => {
          const statsContainer = document.querySelector('.github-stats');
          statsContainer.innerHTML = `
            <p>GitHub Stats:</p>
            <img src="${data.avatar_url}" class="avatar" alt="GitHub Avatar">
            <p>Followers: ${data.followers}</p>
            <p>Following: ${data.following}</p>
            <p>Public Repos: ${data.public_repos}</p>
          `;
        });
    </script>
  </div>
</body>
</html>
