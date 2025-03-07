# Diccionario-LUMA
Un diccionario de un idioma inventado, con una gramática estructurada y a disposición del mundo
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diccionario Español - Luma</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 20px;
            background-color: #f4f4f4;
        }
        h1 {
            color: #333;
        }
        input {
            padding: 10px;
            width: 80%;
            max-width: 300px;
            margin: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 10px 20px;
            border: none;
            background-color: #007BFF;
            color: white;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #0056b3;
        }
        #resultado {
            margin-top: 20px;
            font-size: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <h1>Diccionario Español - Luma</h1>
    <p>Escribe una palabra en español y encuentra su traducción en Luma.</p>
    
    <input type="text" id="buscar" placeholder="Escribe una palabra...">
    <button onclick="traducir()">Buscar</button>
    
    <div id="resultado"></div>

    <script>
        // Diccionario Español - Luma (Extendido con más palabras)
        const diccionario = {
            "casa": "doma",
            "trabajo": "tobá",
            "amigo": "lumo",
            "niño": "funa",
            "mujer": "zara",
            "hombre": "naro",
            "comida": "beka",
            "agua": "fuka",
            "coche": "buto",
            "ropa": "rafa",
            "día": "da",
            "noche": "nara",
            "ciudad": "pura",
            "escuela": "mira",
            "libro": "vero",
            "familia": "huma",
            "sol": "solu",
            "luna": "luna",
            "mar": "mara",
            "montaña": "manta",
            "árbol": "arbo",
            "perro": "peru",
            "gato": "gatu",
            "pájaro": "pano",
            "pez": "pizu",
            "flor": "flura",
            "hoja": "foja",
            "cielo": "sela",
            "tierra": "tira",
            "fuego": "foko",
            "viento": "vintu",
            "camino": "lira",
            "puerta": "pura",
            "ventana": "ventu",
            "mesa": "musa",
            "silla": "sira",
            "papel": "pala",
            "lápiz": "lapu",
            "cuchillo": "nifu",
            "cuchara": "kusa",
            "tenedor": "fuka",
            "plato": "plu",
            "vaso": "vasu",
            "botella": "boti",
            "manzana": "mansa",
            "banana": "baná",
            "naranja": "nara",
            "uva": "uva",
            "pan": "panu",
            "carne": "karnu",
            "pescado": "pisku",
            "verdura": "verdu",
            "azúcar": "suka",
            "sal": "salu",
            "correr": "kore",
            "caminar": "kamina",
            "saltar": "salta",
            "bailar": "baila",
            "cantar": "canta",
            "leer": "lera",
            "escribir": "escri",
            "mirar": "mira",
            "ver": "vira",
            "escuchar": "escu",
            "hablar": "hablu",
            "decir": "diri",
            "pensar": "pensa",
            "soñar": "suña",
            "amar": "ama",
            "odiar": "odia",
            "reír": "rira",
            "llorar": "llora",
            "nacer": "nasa",
            "morir": "mori",
            "vivir": "vive",
            "dormir": "dormu",
            "despertar": "despa",
            "trabajar": "trabaja",
            "descansar": "descansa",
            "jugar": "juga",
            "enseñar": "enseña",
            "aprender": "aprenda",
            "abrir": "abri",
            "cerrar": "cerra",
            "encender": "enci",
            "apagar": "apaga",
            "coger": "koga",
            "soltar": "solta",
            "subir": "subi",
            "bajar": "baja",
            "entrar": "entra",
            "salir": "sali",
            "llegar": "lega",
            "irse": "iru",
            "dar": "dara",
            "recibir": "recibe",
            "comprar": "compra",
            "vender": "vende",
            "esperar": "espera",
            "necesitar": "necesa",
            "buscar": "buska",
            "encontrar": "enku",
            "perder": "perda",
            "robar": "roba",
            "ayudar": "ayuda",
            "conocer": "conoce",
            "saber": "sabe",
            "creer": "crea",
            "dudar": "duda",
            "recordar": "recorda",
            "olvidar": "olvida",
            "llamar": "llama",
            "quedar": "queda",
            "mover": "move",
            "quitar": "quita",
            "poner": "pone",
            "tirar": "tira",
            "romper": "rompe",
            "arreglar": "arregla",
            "mojar": "moja",
            "secar": "seca",
            "sucio": "suka",
            "limpio": "limu",
            "grande": "granda",
            "pequeño": "peku",
            "nuevo": "nuva",
            "viejo": "veja",
            "rápido": "rapida",
            "lento": "lenta",
            "fácil": "fasi",
            "difícil": "difi",
            "caliente": "kali",
            "frío": "frua",
            "bueno": "bona",
            "malo": "mala"
        };

        function traducir() {
            let palabra = document.getElementById("buscar").value.toLowerCase();
            let resultado = document.getElementById("resultado");

            if (diccionario[palabra]) {
                resultado.innerHTML = `La palabra <b>${palabra}</b> en Luma es <b>${diccionario[palabra]}</b>`;
            } else {
                resultado.innerHTML = `La palabra <b>${palabra}</b> no está en el diccionario.`;
            }
        }
    </script>

</body>
</html>
