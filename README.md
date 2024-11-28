<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smiley the Dog</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            overflow-x: hidden;
            background: linear-gradient(135deg, #7D5BA6, #3EC1C1); /* Fondo en violeta y turquesa */
            animation: backgroundAnimation 15s ease infinite; /* Animación para el fondo */
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Hacemos que la página sea un poco más grande */
        }

        @keyframes backgroundAnimation {
            0% {
                background: linear-gradient(135deg, #7D5BA6, #3EC1C1);
            }
            50% {
                background: linear-gradient(135deg, #3EC1C1, #6A4C9C);
            }
            100% {
                background: linear-gradient(135deg, #7D5BA6, #3EC1C1);
            }
        }

        .container {
            text-align: center;
            color: #fff;
            margin-top: 50px;
            max-width: 1200px; /* Para que la página sea más grande */
        }

        h1 {
            font-size: 4em;
            color: #FFD700;
            text-shadow: 3px 3px 10px rgba(0, 0, 0, 0.7);
            animation: fadeInText 1.5s ease-out;
        }

        @keyframes fadeInText {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }

        p {
            font-size: 1.5em;
            color: #FFF;
            line-height: 1.8;
            max-width: 900px;
            margin: 20px auto;
            text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.5);
            animation: slideIn 2s ease-out;
        }

        @keyframes slideIn {
            0% {
                transform: translateX(-100%);
                opacity: 0;
            }
            100% {
                transform: translateX(0);
                opacity: 1;
            }
        }

        .smiley-image {
            width: 300px;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            margin-top: 30px;
            transition: transform 0.3s ease;
            display: inline-block;
        }

        .smiley-image:hover {
            transform: scale(1.1);
        }

        .twitter-logo {
            width: 60px;
            height: 60px;
            background-image: url('https://variety.com/wp-content/uploads/2023/08/X-Logo-Twitter.png');
            background-size: cover;
            background-position: center;
            margin-left: 20px;
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: inline-block;
        }

        .twitter-logo:hover {
            transform: scale(1.1);
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
        }

        a {
            display: inline-block;
            text-decoration: none;
        }

        .solana-tagline {
            font-size: 1.8em;
            color: #FFD700;
            margin-top: 20px;
            font-weight: bold;
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.7);
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Smiley the Dog</h1>
        <p>Smiley is the happiest dog you'll ever meet! With a heart full of joy and a tail that never stops wagging, Smiley is here to brighten your day. Discover more about this adorable pup!</p>
        
        <!-- Imagen de Smiley y logo de Twitter juntos -->
        <div>
            <img src="smiley.jpg" alt="Smiley the Dog" class="smiley-image">
            <a href="https://twitter.com/Smiley" target="_blank">
                <div class="twitter-logo"></div>
            </a>
        </div>

        <!-- Frase relacionada con Solana -->
        <div class="solana-tagline">
            "The Happiest Dog on Solana"
        </div>

    </div>

</body>
</html>
