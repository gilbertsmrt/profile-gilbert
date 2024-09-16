<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profil Saya</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Gaya CSS untuk latar belakang */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            color: #fff;
            text-align: center;
            background: linear-gradient(to right, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.9)), url('TAH APA.jpg') no-repeat center center fixed;
            background-size: cover;
            overflow-x: hidden; /* Mencegah overflow horizontal */
        }

        /* Latar belakang dengan gradien overlay */
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5); /* Gradien gelap di atas gambar */
            z-index: -1;
        }

        /* Gaya CSS untuk welcome */
        .welcome-container {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Mengisi tinggi viewport */
            animation: fadeIn 3s ease-out;
            padding: 0 20px; /* Padding untuk mencegah konten menyentuh tepi layar */
            box-sizing: border-box;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h1 {
            font-size: 3em; /* Menyesuaikan ukuran font untuk perangkat kecil */
            margin: 0;
            color: #fff;
            text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.8);
        }

        /* Gaya CSS untuk tombol */
        .profile-links {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 20px;
        }

        .profile-links a {
            display: inline-block;
            margin: 10px;
            padding: 15px 30px;
            background: linear-gradient(45deg, #ff6f61, #debbff); /* Gradien warna tombol */
            color: #fff;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1em; /* Menyesuaikan ukuran font untuk perangkat kecil */
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, background-color 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }

        .profile-links a:hover {
            transform: scale(1.1);
            background: linear-gradient(45deg, #debbff, #ff6f61);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.4);
        }

        .profile-links a::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 300%;
            height: 300%;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 50%;
            transition: width 0.3s ease, height 0.3s ease;
            transform: translate(-50%, -50%);
            z-index: 0;
        }

        .profile-links a:hover::before {
            width: 0;
            height: 0;
        }

        .profile-links a i {
            margin-right: 10px;
            font-size: 1.5em;
            transition: transform 0.5s ease;
        }

        .profile-links a:hover i {
            transform: scale(1.2) rotate(15deg); /* Animasi ikon */
        }

        /* Gaya CSS untuk halaman tambahan */
        ul {
            list-style-type: none;
            padding: 0;
            margin-top: 20px;
        }

        ul li {
            margin: 10px 0;
        }

        ul li a {
            color: #fff;
            text-decoration: none;
            font-size: 1.1em;
            transition: color 0.3s ease;
        }

        ul li a:hover {
            color: #ff6f61; /* Ubah warna link saat hover */
        }

        /* Gaya CSS untuk footer */
        footer {
            background: rgba(0, 0, 0, 0.7);
            color: #fff;
            padding: 10px 20px;
            position: fixed;
            bottom: 0;
            width: 100%;
            text-align: center;
            font-size: 0.9em;
            box-sizing: border-box;
        }

        footer a {
            color: #ff6f61;
            text-decoration: none;
            font-weight: bold;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="overlay"></div>

    <div class="welcome-container">
        <h1>Haloo Mau ngapain kesini?!</h1>

        <!-- Tombol-tombol profil media sosial -->
        <div class="profile-links">
            <a href="https://www.instagram.com/gilbert_smrt" target="_blank">
                <i class="fab fa-instagram"></i> Instagram
            </a>

            <a href="https://wa.me/+6283100217608" target="_blank">
                <i class="fab fa-whatsapp"></i> WhatsApp
            </a>

            <a href="https://t.me/glsmrtid" target="_blank">
                <i class="fab fa-telegram"></i> Telegram
            </a>

            <a href="https://www.facebook.com/Gilbert Smrt" target="_blank">
                <i class="fab fa-facebook"></i> Facebook
            </a>

            <a href="https://ngl.link/gilbert_smrt1" target="_blank">
                <i class="fab fa-question-circle"></i> NGL
            </a>
        </div>

        <!-- Halaman tambahan -->
        <h2>Halaman Lainnya:</h2>
        <ul>
            <li><a href="tentang.html">Tentang Saya</a></li>
            <li><a href="portofolio.html">Portofolio</a></li>
            <!-- Tambahkan halaman-halaman lain sesuai kebutuhan -->
        </ul>
    </div>

    <footer>
        &copy; 2024 Gilbert Simarmata. Semua hak cipta dilindungi. <a=>Website Anda</a>
    </footer>
</body>
</html>
