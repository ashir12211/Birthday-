<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Premium Birthday Wishes</title>
  <style>
    /* General Styles */
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
    }

    header {
      text-align: center;
      background-color: #ff6f61;
      padding: 20px 0;
    }

    header h1 {
      color: white;
      font-size: 3rem;
      margin: 0;
    }

    .banner img {
      width: 100%;
      max-height: 300px;
      object-fit: cover;
    }

    main {
      padding: 20px;
    }

    .wishes {
      text-align: center;
      margin-bottom: 40px;
    }

    .wish-container {
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      display: inline-block;
    }

    #wish-text {
      font-size: 1.2rem;
      margin-bottom: 20px;
    }

    #generate-wish {
      background-color: #ff6f61;
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 1rem;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    #generate-wish:hover {
      background-color: #ff4a3d;
    }

    .gallery {
      text-align: center;
    }

    .image-grid {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
    }

    .image-grid img {
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #333;
      color: white;
      margin-top: 40px;
    }

    footer p {
      margin: 0;
    }
  </style>
</head>
<body>
  <header>
    <div class="banner">
      <img src="https://via.placeholder.com/1200x300" alt="Birthday Banner">
      <h1>Happy Birthday!</h1>
    </div>
  </header>

  <main>
    <section class="wishes">
      <h2>Birthday Wishes</h2>
      <div class="wish-container">
        <p id="wish-text">Click the button to generate a birthday wish!</p>
        <button id="generate-wish">Generate Wish</button>
      </div>
    </section>

    <section class="gallery">
      <h2>Birthday Gallery</h2>
      <div class="image-grid">
        <img src="https://via.placeholder.com/200" alt="Birthday Image 1">
        <img src="https://via.placeholder.com/200" alt="Birthday Image 2">
        <img src="https://via.placeholder.com/200" alt="Birthday Image 3">
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Premium Birthday Wishes. All rights reserved.</p>
  </footer>

  <script>
    // JavaScript for generating random birthday wishes
    const wishes = [
      "Wishing you a day filled with happiness and a year filled with joy. Happy Birthday!",
      "May your birthday be as special as you are. Cheers to another year of amazing adventures!",
      "Sending you smiles for every moment of your special day. Have a wonderful birthday!",
      "Hope your birthday is as sweet as cake and as bright as candles. Happy Birthday!",
      "Another year older, wiser, and more fabulous. Happy Birthday!",
    ];

    const wishText = document.getElementById("wish-text");
    const generateWishButton = document.getElementById("generate-wish");

    generateWishButton.addEventListener("click", () => {
      const randomWish = wishes[Math.floor(Math.random() * wishes.length)];
      wishText.textContent = randomWish;
    });
  </script>
</body>
</html>
