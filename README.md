<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Komik Web Sayfası</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Hoş Geldin, Komedi Sever!</h1>
    </header>
    <main>
        <section>
            <h2>Gülme Garanti!</h2>
            <p>Bu siteyi açtığın için seni tebrik ediyorum!</p>
            <p>Çünkü burada gülmek zorundasın!</p>
            <button onclick="showJoke()">Bir Şaka Göster!</button>
            <p id="joke"></p>
        </section>
    </main>
    <footer>
        <p>Telif hakkı &copy; 2024, Gülümse ve Devam Et!</p>
    </footer>
    <script>
        function showJoke() {
            const jokes = [
                "Neden bilgisayar denize düşer? Çünkü suya girmeyi çok sever!",
                "Bir programcı, tuvalette ne yapar? Kodu temizler!",
                "Neden kitaplar soğuk olur? Çünkü sayfaları var!",
            ];
            const randomIndex = Math.floor(Math.random() * jokes.length);
            document.getElementById('joke').innerText = jokes[randomIndex];
        }
    </script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #e0f7fa;
}

header {
    background: #00796b;
    color: white;
    padding: 10px 0;
    text-align: center;
}

main {
    padding: 20px;
    text-align: center;
}

h2 {
    color: #00796b;
}

button {
    background-color: #ffab00;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 16px;
}

button:hover {
    background-color: #ff8f00;
}

footer {
    text-align: center;
    padding: 10px 0;
    background: #00796b;
    color: white;
    position: absolute;
    bottom: 0;
    width: 100%;
}

