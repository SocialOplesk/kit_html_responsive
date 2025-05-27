# SOCIAL OPLESK
### 💼 KIT 
<br/>

## ⚡️ Kit media query⚡️
<br/> 

## 🏆 K-1 (MEDIA QUERY)

Media query 
```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>K-1</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }

        .box {
            background-color: #3498db; /* Azul por defecto */
            color: white;
            padding: 20px;
            text-align: center;
            border-radius: 8px;
            width: 80%;
            max-width: 500px;
            font-size: 16px;
        }

        /* Única Media Query: max-width (pantallas hasta 600px) */
        @media screen and (max-width: 600px) {
            .box {
                background-color: #e74c3c; /* Rojo */
                font-size: 14px;
                border-radius: 0; /* Bordes rectos */
            }
        }
    </style>
</head>
<body>
    <div class="box">
        <h1>¡Prueba de Media Query!</h1>
        <p>Redimensiona la ventana para ver los cambios.</p>
    </div>
</body>
</html>
```


## 🏆 K-2 (MEDIA QUERIES)

Media query 
```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>K-2</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }

        .box {
            background-color: #3498db;
            color: white;
            padding: 20px;
            text-align: center;
            border-radius: 8px;
            width: 80%;
            max-width: 500px;
            font-size: 16px;
        }

        /* Media Query 1: max-width (pantallas pequeñas, hasta 600px) */
        @media screen and (max-width: 600px) {
            .box {
                background-color: #e74c3c; /* Rojo */
                font-size: 14px;
                padding: 15px;
            }
        }

        /* Media Query 2: min-width (pantallas grandes, desde 900px) */
        @media screen and (min-width: 900px) {
            .box {
                background-color: #2ecc71; /* Verde */
                font-size: 20px;
                padding: 30px;
            }
        }

        /* Media Query 3: orientation (pantallas en modo horizontal) */
        @media screen and (orientation: landscape) {
            .box {
                background-color: #3355ff; /* Azul */ 
                width: 60%;
                border: 3px solid #fff;
            }
        }
    </style>
</head>
<body>
    <div class="box">
        <h1>¡Prueba de Media Queries!</h1>
        <p>Redimensiona la ventana o rota el dispositivo para ver los cambios.</p>
    </div>
</body>
</html>
```

## 🏆 K-3 (MAX AND MIN)

Media query 
```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>K-3</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }

        .box {
            background-color: #3498db; /* Azul por defecto */
            color: white;
            padding: 20px;
            text-align: center;
            border-radius: 8px;
            width: 80%;
            max-width: 500px;
            font-size: 16px;
        }

        /* Única Media Query: min-width y max-width combinados con AND */
        @media screen and (min-width: 600px) and (max-width: 900px) {
            .box {
                background-color: #f39c12; /* Naranja */
                border: 2px dashed #fff;
                font-style: italic;
            }
        }
    </style>
</head>
<body>
    <div class="box">
        <h1>¡Prueba de Media Query!</h1>
        <p>Redimensiona la ventana para ver los cambios.</p>
    </div>
</body>
</html>
```

## 🏆 K-4 (MEDIA QUERY + ACTION)

Media query 
```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>k-4</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .navbar {
            background-color: #333;
            padding: 15px;
        }

        .nav-list {
            list-style: none;
            display: flex;
            justify-content: center;
        }

        .nav-list li {
            margin: 0 20px;
        }

        .nav-list a {
            color: white;
            text-decoration: none;
            font-size: 18px;
        }

        .nav-list a:hover {
            color: #ddd;
        }

        .menu-toggle {
            display: none;
        }

        .menu-checkbox {
            display: none;
        }

        .menu-toggle-label {
            display: none;
            color: white;
            font-size: 24px;
            cursor: pointer;
            text-align: right;
            padding: 10px;
        }

        /* Media Query para pantallas menores a 768px */
        @media screen and (max-width: 768px) {
            .menu-toggle-label {
                display: block;
            }

            .nav-list {
                display: none;
                flex-direction: column;
                width: 100%;
                background-color: #333;
                position: absolute;
                top: 60px;
                left: 0;
            }

            .menu-checkbox:checked ~ .nav-list {
                display: flex;
            }

            .nav-list li {
                margin: 10px 0;
                text-align: center;
            }
        }

        /* Media Query para pantallas menores a 480px */
        @media screen and (max-width: 480px) {
            .nav-list a {
                font-size: 16px;
            }

            .menu-toggle-label {
                font-size: 20px;
            }
        }
    </style>
</head>
<body>
    <nav class="navbar">
        <input type="checkbox" id="menu-toggle" class="menu-checkbox">
        <label for="menu-toggle" class="menu-toggle-label">☰</label>
        <ul class="nav-list">
            <li><a href="#home">Inicio</a></li>
            <li><a href="#about">Acerca</a></li>
            <li><a href="#services">Servicios</a></li>
            <li><a href="#contact">Contacto</a></li>
        </ul>
    </nav>
</body>
</html>
```

---
<h3 align="center">SOCIAL OPLESK</h3>



