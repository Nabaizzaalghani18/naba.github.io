
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Registrasi</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
    font-family: 'Arial', sans-serif;
    background: linear-gradient(135deg, #74ebd5, #acb6e5);
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.container {
    width: 400px;
    padding: 30px;
    background: white;
    border-radius: 15px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    text-align: center;
}
h1 {
    margin-bottom: 20px;
    color: #333;
}
.form-group {
    margin-bottom: 20px;
}
label {
    display: block;
    margin-bottom: 5px;
    color: #555;
}
input[type="text"],
input[type="email"],
input[type="password"],
input[type="date"] {
    width: 100%;
    padding: 15px;
    border: 2px solid #ddd;
    border-radius: 10px;
    box-sizing: border-box;
    transition: border-color 0.3s;
}
input[type="text"]:focus,
input[type="email"]:focus,
input[type="password"]:focus,
input[type="date"]:focus {
    border-color: #74ebd5;
    outline: none;
}
.gender-options {
    display: flex;
    justify-content: space-around;
}
button {
    width: 100%;
    padding: 15px;
    background-color: #74ebd5;
    color: white;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
}
button:hover {
    background-color: #3bb78f;
}
p {
    margin-top: 20px;
}
a {
    color: #74ebd5;
    text-decoration: none;
    transition: color 0.3s;
}
a:hover {
    color: #3bb78f;
}
    </style>
</head>
<body>
    <div class="container">
        <h1>Registrasi Akun</h1>
        <form action="#" method="POST">
            <div class="form-group">
                <label for="nama">Nama Lengkap</label>
                <input type="text" id="nama" name="nama" required>
            </div>
            <div class="form-group">
                <label for="email">Email</label>
                <input type="email" id="email" name="email" required>
            </div>
            <div class="form-group">
                <label for="password">Kata Sandi</label>
                <input type="password" id="password" name="password" required>
            </div>
            <div class="form-group">
                <label for="konfirmasi-password">Konfirmasi Kata Sandi</label>
                <input type="password" id="konfirmasi-password" name="konfirmasi-password" required>
            </div>
            <div class="form-group">
                <label>Jenis Kelamin</label>
                <div class="gender-options">
                    <label>
                        <input type="radio" name="gender" value="Laki-laki" required>
                        Laki-laki
                    </label>
                    <label>
                        <input type="radio" name="gender" value="Perempuan" required>
                        Perempuan
                    </label>
                </div>
            </div>
            <div class="form-group">
                <label for="tanggal-registrasi">Tanggal Registrasi</label>
                <input type="date" id="tanggal-registrasi" name="tanggal-registrasi" required>
            </div>
            <button type="submit">Daftar</button>
        </form>
        <p>Sudah punya akun? <a href="#">Masuk di sini</a></p>
    </div>
</body>
</html>
