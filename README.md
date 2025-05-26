in# The-real-world-by-Dhruv
The things present in the world 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>The Real World - Home</title>
<style>
  body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #fff;
    color: #000;
  }
  header {
    background: #000;
    color: red;
    padding: 15px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  header h1 {
    margin: 0;
    font-weight: bold;
    font-size: 24px;
  }
  nav a {
    color: red;
    text-decoration: none;
    margin-left: 20px;
    font-weight: 600;
  }
  nav a:hover {
    text-decoration: underline;
  }
  .slider {
    margin: 20px auto;
    max-width: 600px;
    overflow: hidden;
    border: 2px solid red;
    border-radius: 8px;
  }
  .slides {
    display: flex;
    transition: transform 0.5s ease-in-out;
  }
  .slides img {
    width: 600px;
    height: 400px;
    object-fit: cover;
  }
  footer {
    margin-top: 40px;
    padding: 10px 20px;
    text-align: center;
    color: #444;
    border-top: 1px solid #eee;
  }
  @media(max-width: 640px) {
    .slides img {
      width: 100%;
      height: auto;
    }
    .slider {
      max-width: 100%;
    }
  }
</style>
</head>
<body>

<header>
  <h1>The Real World</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">Reels</a>
    <a href="#">Post</a>
    <a href="#">Login</a>
  </nav>
</header>

<section class="slider" aria-label="Image Slider">
  <div class="slides" id="slides">
    <img src="https://picsum.photos/id/1015/600/400" alt="Nature Image 1" />
    <img src="https://picsum.photos/id/1016/600/400" alt="Nature Image 2" />
    <img src="https://picsum.photos/id/1018/600/400" alt="Nature Image 3" />
  </div>
</section>

<footer>
  Owned by Dhruv Tiwari
</footer>

<script>
  const slides = document.getElementById('slides');
  let index = 0;
  const total = slides.children.length;

  setInterval(() => {
    index++;
    if(index >= total) index = 0;
    slides.style.transform = `translateX(${-index * 600}px)`;
  }, 3000);
</script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Reels - The Real World</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #fff;
      color: #000;
    }
    header {
      background: #000;
      color: red;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
      font-size: 24px;
    }
    nav a {
      color: red;
      text-decoration: none;
      margin-left: 20px;
      font-weight: 600;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .reels-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      padding: 20px;
    }
    .reel {
      border: 2px solid red;
      border-radius: 10px;
      overflow: hidden;
      background-color: #000;
    }
    video {
      width: 100%;
      height: auto;
      display: block;
    }
    footer {
      margin-top: 20px;
      padding: 10px 20px;
      text-align: center;
      color: #444;
      border-top: 1px solid #eee;
    }
  </style>
</head>
<body>

<header>
  <h1>The Real World</h1>
  <nav>
    <a href="index.html">Home</a>
    <a href="reels.html">Reels</a>
    <a href="post.html">Post</a>
    <a href="login.html">Login</a>
  </nav>
</header>

<main class="reels-grid">
  <div class="reel">
    <video src="https://www.w3schools.com/html/mov_bbb.mp4" controls></video>
  </div>
  <div class="reel">
    <video src="https://www.w3schools.com/html/movie.mp4" controls></video>
  </div>
  <div class="reel">
    <video src="https://www.w3schools.com/html/mov_bbb.mp4" controls></video>
  </div>
  <!-- Add more video reels below -->
</main>

<footer>
  Owned by Dhruv Tiwari
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Post - The Real World</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #fff;
      color: #000;
    }
    header {
      background: #000;
      color: red;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
      font-size: 24px;
    }
    nav a {
      color: red;
      text-decoration: none;
      margin-left: 20px;
      font-weight: 600;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .post-container {
      max-width: 800px;
      margin: 30px auto;
      padding: 0 20px;
    }
    .post-container img {
      width: 100%;
      border-radius: 10px;
      border: 2px solid red;
    }
    .post-title {
      font-size: 28px;
      font-weight: bold;
      color: red;
      margin-top: 20px;
    }
    .post-content {
      margin-top: 15px;
      font-size: 18px;
      line-height: 1.6;
    }
    footer {
      margin-top: 40px;
      padding: 10px 20px;
      text-align: center;
      color: #444;
      border-top: 1px solid #eee;
    }
  </style>
</head>
<body>

<header>
  <h1>The Real World</h1>
  <nav>
    <a href="index.html">Home</a>
    <a href="reels.html">Reels</a>
    <a href="post.html">Post</a>
    <a href="login.html">Login</a>
  </nav>
</header>

<div class="post-container">
  <img src="https://picsum.photos/id/1025/800/400" alt="Post Image">
  <h2 class="post-title">Welcome to The Real World Blog</h2>
  <div class="post-content">
    <p>
      This is a sample blog post to demonstrate the design and structure of your "Post" page. You can write about your thoughts, ideas, news, or anything you want to share with your audience here.
    </p>
    <p>
      Add more posts by creating multiple pages, or connect this to a database or CMS later if you want dynamic content. For now, this is a clean and responsive static blog layout.
    </p>
  </div>
</div>

<footer>
  Owned by Dhruv Tiwari
</footer>

</body>
</html>
