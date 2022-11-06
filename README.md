<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Navbar</title>
    <link rel="stylesheet" href="./Navbar.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Raleway', sans-serif;
        }

        .container {
            height: 100vh;
            width: 100%;
            background-image: linear-gradient(-45deg, #F9ED69, #F08A5D, #B83B5E, #6A2C70);
            animation: NavAnim 10s ease infinite;
            background-size: 400% 400%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            gap: 10px;
            color: white;
        }


        @keyframes NavAnim {
            0% {
                background-position: 0% 50%;
            }

            50% {
                background-position: 100% 50%;
            }

            100% {
                background-position: 0% 50%;
            }
        }

        #welcome {
            font-size: 60px;
            font-weight: 500;
        }

        #content {
            font-size: 25px;
        }

        @media (max-width:320px) {
            #welcome {
                font-size: 30px;
            }

            #content {
                font-size: 12.5px;
            }
        }
    </style>
</head>

<body>
    <div class="container">
        <h1 id="welcome">Welcome!</h1>
        <p id="content">Its Mohit Here.</p>
    </div>
</body>
<script src="./Navbar.js"></script>

</html>
