# Projek-Web-Trisma
Membuat 1 halaman web sederhana
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trisma Nurdiawati</title>
    <style>
        * {
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            margin: 0;
            display: grid;
            place-items: center;
            padding: 24px;
            background: #eaf3f8;
            color: #233746;
            font-family: Arial, sans-serif;
        }

        main {
            width: min(100%, 620px);
            padding: 36px;
            border-radius: 18px;
            background: #ffffff;
            box-shadow: 0 12px 32px rgb(35 55 70 / 12%);
        }

        h1 {
            margin-top: 0;
            color: #176b87;
        }

        .ilustrasi {
            display: block;
            width: 100%;
            height: auto;
            margin: 20px 0;
            border-radius: 12px;
        }

        p {
            line-height: 1.7;
        }

        button {
            padding: 12px 18px;
            border: 0;
            border-radius: 8px;
            background: #176b87;
            color: #ffffff;
            font: inherit;
            cursor: pointer;
        }

        button:hover {
            background: #10546b;
        }

        #waktu {
            min-height: 1.7em;
            color: #176b87;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <main>
        <h1>Halo, Trisma Nurdiawati!</h1>
        <figure class="foto profile">
            <img src="images/IMG-20260409-WA0303.jpg" width="335" height="450" alt="Potret Trisma Nurdiawati, seorang perempuan muda yang tersenyum santai ke arah kamera. Dia mengenakan pakaian kasual dan terlihat rileks, dengan latar belakang yang lembut dan sederhana. Suasana foto terasa hangat, bersahabat, dan nyaman." />
        </figure>
        <p>Selamat datang di halaman sederhana saya. Halaman ini dibuat sebagai latihan dasar HTML, CSS, dan JavaScript.</p>
        <p>Saya senang mempelajari hal-hal baru, terutama teknologi dan cara membuat website yang bermanfaat.</p>
        <p>Semoga halaman kecil ini menjadi langkah awal untuk membuat lebih banyak karya digital yang menarik.</p>
        <button type="button" id="tombol-waktu">Tampilkan tanggal dan waktu</button>
        <p id="waktu" aria-live="polite"></p>
    </main>
    <script>
        document.getElementById("tombol-waktu").addEventListener("click", function () {
            document.getElementById("waktu").textContent =
                "Sekarang: " + new Date().toLocaleString("id-ID");
        });
    </script>
</body>
</html>
