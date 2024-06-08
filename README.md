<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AKU DAN ENGKAU</title>
    <link rel="stylesheet" href="style.css">
    <style>
        body {
    font-family: 'Comic Sans MS', cursive, sans-serif;
    background-color: #ffebcd;
    color: #333;
    margin: 0;
    padding: 0;
    overflow: hidden;
}
header {
    background-color: #4a0eba;
    color: white;
    padding: 10px 0;
    text-align: center;
    position: relative;
    z-index: 1;
}
main {
    padding: 20px;
    max-width: 800px;
    margin: auto;
    position: relative;
    z-index: 1;
    text-align: center;
}
img {
    max-width: auto;
    height: 400px;
    border-radius: 8px;
}
.description {
    margin-top: 20px;
    animation: fadeIn 3s;
}
footer {
    background-color: #1e3bbc;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
    z-index: 1;
}
@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}
.heart {
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: rgb(78, 123, 219);
    transform: rotate(45deg);
    animation: float 5s infinite;
}
.heart::before, .heart::after {
    content: '';
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: rgb(64, 133, 206);
    border-radius: 50%;
}
.heart::before {
    top: -10px;
    left: 0;
}
.heart::after {
    top: 0;
    left: -10px;
}
@keyframes float {
    0% { transform: translateY(0) rotate(45deg); opacity: 1; }
    100% { transform: translateY(-200px) rotate(45deg); opacity: 0; }
}
audio {
    display: none;
}
    </style>
</head>
<body>
    <header>
        <h1>Aku Dan Engkau</h1>
    </header>
    <main>
        <section>
            <h2>Kepada: My Sweetheart</h2>
            <img src="WhatsApp Image 2024-06-08 at 16.36.07_25296027.jpg" alt="Cute Image">
            <div class="description">
                <p>Sayangku, kamu adalah alasan aku tersenyum setiap hari. Kehadiranmu membuat hidupku sempurna dan penuh warna. Aku sangat beruntung memiliki kamu dalam hidupku. Aku mencintaimu lebih dari kata-kata yang bisa diungkapkan.</p>
                <p>Bersamamu adalah anugerah terindah, dan aku ingin selalu berada di sisimu selamanya. Kamu adalah bintang yang menerangi malam-malamku dan sinar matahari yang menghangatkan hariku.</p>
                <p>I love you to the moon and back!</p>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Oleh Hegal Rey</p>
    </footer>
    <audio autoplay loop>
        <source src="DJ Snake - Let Me Love You ft. Justin Bieber (Lyrics).mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
    <script>
        function createHeart() {
            const heart = document.createElement('div');
            heart.className = 'heart';
            heart.style.top = Math.random() * 100 + 'vh';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 2 + 3 + 's';
            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 5000);
        }

        setInterval(createHeart, 500);
    </script>
</body>
</html>
