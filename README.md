<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/boxicons@latest/css/boxicons.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <title>Luxury Cars</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: #f4f4f4;
            color: #333;
            line-height: 1.6;
        }

        /* Header */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 10%;
            background: #fff;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        .logo {
            font-size: 1.5rem;
            color: #333;
            text-decoration: none;
        }

        .navigation {
            list-style: none;
            display: flex;
        }

        .navigation li {
            margin-left: 20px;
        }

        .navigation a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s;
        }

        .navigation a:hover {
            color: #007bff;
        }

        .header-icons {
            display: flex;
            align-items: center;
        }

        .header-icons i {
            font-size: 1.2rem;
            margin-left: 20px;
            cursor: pointer;
        }

        #menu {
            display: none;
        }

        /* Sections */
        .section {
            display: none;
            padding: 50px 10%;
        }

        .active {
            display: block;
        }

        /* Home Section */
        .home {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 50px 10%;
            background: linear-gradient(135deg, #111, #444);
            color: #fff;
        }

        .home-img img {
            width: 450px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .home-text {
            max-width: 500px;
        }

        .home-text h1 {
            font-size: 3rem;
            line-height: 1.2;
            margin-bottom: 20px;
        }

        .home-text h5 {
            font-size: 1.5rem;
            margin-bottom: 20px;
        }

        .home-text h3 {
            font-size: 2rem;
            margin-bottom: 20px;
        }

        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: #007bff;
            color: #fff;
            border-radius: 5px;
            text-decoration: none;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #0056b3;
        }

        /* Main Section */
        .main {
            display: flex;
            justify-content: center;
            padding: 20px 10%;
        }

        .row {
            margin: 0 10px;
        }

        .row img {
            width: 100px;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .row img:hover {
            transform: scale(1.1);
        }

        /* Media Queries */
        @media (max-width: 768px) {
            .navigation {
                display: none;
                flex-direction: column;
                background: #fff;
                position: absolute;
                top: 70px;
                right: 10%;
                width: 200px;
                box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            }

            .navigation.open {
                display: flex;
            }

            .home {
                flex-direction: column;
                text-align: center;
            }

            .home-img img {
                width: 100%;
            }

            .home-text h1 {
                font-size: 2rem;
            }

            .home-text h5, .home-text h3 {
                font-size: 1.2rem;
            }

            #menu {
                display: block;
            }
        }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo"><i class='bx bx-car'></i>Luxury Cars</a>
        <ul class="navigation">
            <li><a href="#" onclick="showSection('home')">Overview</a></li>
            <li><a href="#" onclick="showSection('store')">Conheça a loja</a></li>
            <li><a href="#" onclick="showSection('history')">Nossa história</a></li>
            <li><a href="#" onclick="showSection('contact')">Contato</a></li>
        </ul>
        <div class="header-icons">
            <i class='bx bx-cart'></i>
            <div id="menu"><i class='bx bx-menu'></i></div>
        </div>
    </header>

    <section id="home" class="section home active">
        <div class="home-img">
            <img src="C:\Users\Guilherme Rodrigues\Downloads\kisspng-2017-porsche-911-2018-porsche-911-car-2015-porsche-5aee8ad78c8029.6806278515255825515755.png" class="one" alt="Luxury Car" style="width: 120%; margin-left: -130px;">
        </div>
        <div class="home-text">
            <h1>Luxury <br> Cars</h1>
            <h5>O ápice da elegancia automativa</h5>
            <h3>R$15,000.000</h3>
            <a href="#" class="btn">Shop Now</a>
        </div>
    </section>
    

    <section id="store" class="section">
        <h2>Conheça a loja</h2>
        <p>Em nosso site, você encontrará a mais refinada seleção de carros de luxo, onde cada veículo é uma obra-prima de design, desempenho e tecnologia. Nossa coleção exclusiva é meticulosamente escolhida para atender aos gostos mais exigentes, proporcionando uma experiência incomparável de sofisticação e prazer ao dirigir.</p>
        <h3>A Experiência Suprema</h3>
        <p>Cada veículo em nossa coleção não é apenas um carro, mas uma expressão de arte e performance. Com acabamentos impecáveis, materiais de altíssima qualidade e tecnologias inovadoras, nossos carros de luxo proporcionam uma experiência de condução inigualável. Visite-nos e descubra o verdadeiro significado de luxo automotivo.</p>
        <h3>Agende um Test Drive</h3>
        <p>Experimente a exclusividade e o desempenho de nossos carros de luxo em um test drive. Nossos consultores especializados estão à disposição para ajudá-lo a escolher o modelo perfeito que atenda às suas expectativas e desejos.</p>
        <p>Entre em contato conosco para mais informações e descubra como é estar no volante do carro dos seus sonhos.</p>
    </section>

    <section id="history" class="section">
        <h2>Nossa história</h2>
        <p>Somos uma concessionária de carros fundada por três colegas de sala que compartilhavam a paixão por automóveis. Nossa história começou em uma pequena garagem e, com muito trabalho e dedicação, nos tornamos uma das principais concessionárias da região.</p>
    </section>

    <section id="contact" class="section">
        <h2>Contato</h2>
        <p>Email: contato@concessionariacarros.com

            <p>Telefone (Recepção): (11) 1234-5678</p>
            
            Telefone (SAC): (11) 8765-4321.</p>
    </section>

    <div class="main">
        <div class="row"><img src="C:\Users\Guilherme Rodrigues\Downloads\9464a1aa6effe666c1864fe8149e2114.png" onclick="slider('gratis.png')" alt="Car Thumbnail 1"></div>
        <div class="row"><img src="C:\Users\Guilherme Rodrigues\Downloads\05aa768491d6a322a4dcd4d8064cc42b.png" onclick="slider('car2.png')" alt="Car Thumbnail 2"></div>
        <div class="row"><img src="C:\Users\Guilherme Rodrigues\Downloads\c22d1f9a7af1211b8a0eb688387c8954.png" onclick="slider('car3.png')" alt="Car Thumbnail 3"></div>
    </div>

    <script>
        function slider(anything) {
            document.querySelector('.one').src = anything;
        }
        let menu = document.querySelector('#menu');
        let navigation = document.querySelector('.navigation');
        menu.onclick = () => {
            menu.classList.toggle('bx-x');
            navigation.classList.toggle('open');
        }

        function showSection(sectionId) {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => section.classList.remove('active'));
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
    
</body>
</html>
