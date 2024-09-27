<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Terima Kasih!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f8ff;
            text-align: center;
            padding: 50px;
            overflow: hidden;
            height: 100vh;
            margin: 0;
        }

        h1 {
            font-size: 3rem;
            color: #ff6347;
            animation: fadeIn 2s ease-in-out;
        }

        p {
            font-size: 1.5rem;
            color: #666;
            animation: fadeIn 4s ease-in-out;
        }

        .balloon {
            position: absolute;
            bottom: -100px;
            background-color: #ff6347;
            width: 30px;
            height: 50px;
            border-radius: 50%;
            animation: float 7s ease-in infinite;
        }

        .balloon:nth-child(odd) {
            background-color: #ffcc5c;
        }

        .balloon:nth-child(even) {
            background-color: #88d8b0;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes float {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(-120vh);
            }
        }

        button {
            margin-top: 30px;
            padding: 10px 20px;
            background-color: #ff6347;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.2rem;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #ff4500;
        }
    </style>
</head>
<body>

    <h1>Terima Kasih!</h1>
    <p>Terima kasih telah mengisi survei ini. 😊</p>

    <!-- Balon Animasi -->
    <div class="balloon" style="left: 10%; animation-duration: 6s;"></div>
    <div class="balloon" style="left: 20%; animation-duration: 8s;"></div>
    <div class="balloon" style="left: 30%; animation-duration: 7s;"></div>
    <div class="balloon" style="left: 50%; animation-duration: 9s;"></div>
    <div class="balloon" style="left: 70%; animation-duration: 6s;"></div>
    <div class="balloon" style="left: 90%; animation-duration: 8s;"></div>

    <button onclick="goToSecret()">Lihat Pesan Rahasia</button>

    <script>
        function goToSecret() {
            window.location.href = "halaman_rahasia.html"; // Ubah ke URL halaman kedua
        }
    </script>

</body>
</html>
