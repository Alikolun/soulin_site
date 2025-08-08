<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Aşklar Sitesi</title>
<style>
  body {
    margin: 0; padding: 20px;
    background: #ffc0cb;
    font-family: 'Arial', sans-serif;
    color: #fff;
    text-align: center;
    position: relative;
    overflow-x: hidden;
  }
  body::before {
    content: "♥ ♥ ♥ ♥ ♥ ♥ ♥ ♥ ♥ ♥";
    position: fixed;
    top: 10px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 50px;
    color: rgba(255, 0, 50, 0.15);
    user-select: none;
    pointer-events: none;
    animation: floatHearts 10s linear infinite;
  }
  @keyframes floatHearts {
    0% { transform: translateX(-50%) translateY(0); }
    100% { transform: translateX(-50%) translateY(-300px);}
  }
  h1 {
    margin-bottom: 20px;
    font-size: 48px;
    text-shadow: 0 0 5px #c70039;
  }
  .container {
    max-width: 900px;
    margin: 0 auto;
  }
  .videos, .photos, .texts {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
    margin-bottom: 30px;
  }
  video {
    width: 45%;
    max-width: 400px;
    border-radius: 15px;
    box-shadow: 0 0 10px #c70039;
  }
  img {
    width: 45%;
    max-width: 400px;
    border-radius: 15px;
    box-shadow: 0 0 10px #c70039;
  }
  textarea {
    width: 45%;
    max-width: 400px;
    min-height: 120px;
    border-radius: 15px;
    border: none;
    padding: 10px;
    font-size: 16px;
    resize: none;
    box-shadow: 0 0 10px #c70039;
    background: rgba(255,255,255,0.15);
    color: white;
  }
  textarea::placeholder {
    color: #ffc0cb;
  }
  label {
    display: block;
    margin-bottom: 8px;
    font-weight: bold;
    text-shadow: 0 0 3px #900;
  }
</style>
</head>
<body>
  <h1>Aşklar Sitesi</h1>
  <div class="container">

    <section class="videos">
      <video controls src="video1.mp4" type="video/mp4" ></video>
      <video controls src="video2.mp4" type="video/mp4" ></video>
      <video controls src="video3.mp4" type="video/mp4" ></video>
      <video controls src="video4.mp4" type="video/mp4" ></video>
    </section>

    <section class="photos">
      <img src="photo1.jpg" alt="Fotoğraf 1" />
      <img src="photo2.jpg" alt="Fotoğraf 2" />
      <img src="photo3.jpg" alt="Fotoğraf 3" />
      <img src="photo4.jpg" alt="Fotoğraf 4" />
    </section>

    <section class="texts">
      <label for="text1">Şiir 1 (max 300 karakter):</label>
      <textarea id="text1" maxlength="300" placeholder="Şiirini buraya yaz..."></textarea>

      <label for="text2">Şiir 2 (max 300 karakter):</label>
      <textarea id="text2" maxlength="300" placeholder="Şiirini buraya yaz..."></textarea>

      <label for="text3">Mektup (max 300 karakter):</label>
      <textarea id="text3" maxlength="300" placeholder="Mektubunu buraya yaz..."></textarea>
    </section>

  </div>
</body>
</html>
