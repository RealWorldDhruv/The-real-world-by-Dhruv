# The-real-world-by-Dhruv
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
