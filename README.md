# Hugolopes
sitecomeço
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mig Instrumentos</title>
     <link rel="stylesheet" href="./styles/globals.css">
   
</head>
<body>

    <div class="navbar">
        <div class="header-inner-content">
            <h1 class="logo">Mig<span>Instrumentos🎷</span></h1>
        
            <nav class="nav-menu">
                <ul>
                    <li>Home</li>
                    <li><a href="produtos.html">Produtos</a></li>
                    <li><a href="cadastro-login.html">login</a></li>
                    <li>Informática</li>
                    <li>Instrumento</li>
                </ul>
            </nav>
   
            <div class="nav-icon-container">
                <img src="images/cart.png" alt="Carrinho de Compras" />
                <img src="images/menu.png" alt="Menu" class="menu-button" />
            </div>
        </div>
    </div>

    <header>
        <div class="header-inner-content">
            <div class="header-bottom-side">
                <div class="header-bottom-side-left">
                    <h2>Compre seu instrumento ideal ao seu trabalho</h2>
                    <p>
                        Quando as palavras falham, a música fala – ela tem o poder de tocar a alma e transformar o coração."
                    </p>
                    <a href="produtos.html">
                        <button>Ver agora &#8594;</button>
                      </a>
                </div>
                <div class="header-bottom-side-right"></div>
                <img src="images/logotipo2.jpg" alt="Instrumentos" />
            </div>
        </div>
    </header>

    
        
    

    <script>
     
        const menuButton = document.querySelector(".menu-button");
        const navMenu = document.querySelector(".nav-menu");

        
        menuButton.addEventListener("click", function() {
            navMenu.classList.toggle("show-menu"); 
        });
    </script>
    
</body>




<div class=contactos>
    <div>
        <h1>Contatos</h1>
         <p>telefone:6192230593 📞</p>
        <p>email:hugo1230lopess@gmail.com📧</p>
        <p>endereço:casa 26 a lote b🏠</p>
    </div>
</div>

</html>


css 





* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: rgb(131, 130, 130)
}

/* Navegação */
.navbar {
    background-color: #1a1a46;
    padding: 1rem;
    position: sticky;
    top: 0;
    box-shadow: 10px 8px 10px #2c2c2c;
    z-index: 99;
}

.navbar > div {
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: relative;
}

.logo {
    color: rgb(216, 216, 216);
}

nav ul {
    display: flex;
    list-style: none;
    align-items: center;
    margin: 0;
}

.nav-icon-container {
    display: flex;
    align-items: center;
}

.nav-icon-container img {
    width: 30px;
    cursor: pointer;
}

.nav-icon-container img:first-child {
    margin-right: 1rem;
}

/* Esconde o menu por padrão */
.nav-menu {
    display: none;  /* Menu escondido por padrão em telas pequenas */
}

/* Exibe o menu quando a classe 'show-menu' é adicionada */
.show-menu {
    display: block;  /* Torna o menu visível */
}

/* Itens do menu */
nav ul li {
    color: rgb(240, 248, 255);
    margin-right: 1.5rem;
    cursor: pointer;
}

nav ul li:hover {
    transform: translateY(-5px);
    transition: all 0.2s;
    font-weight: bold;
}


.menu-button {
    display: block; 
}

header {
    background-image: radial-gradient(circle, #dddddd, #a7a5a5);
}

.header-bottom-side {
    display: flex;
    align-items: center;
    justify-self: center;
    padding: 1rem;
}

.header-bottom-side-left {
    height: 100%;
    flex-basis: 50%;
}

.header-bottom-side-left h2 {
    font-size: 3.2rem;
    margin-bottom: 1.5rem;
}

.header-bottom-side-left p {
    line-height: 1.5rem;
    margin-bottom: 1.5rem;
}

.header-bottom-side-left button {
    background-color: #1515f1;
    border: none;
    cursor: pointer;
    padding: 0.8rem 3.8rem;
    border-radius: 9999px;
    color: #fff;
    font-weight: 500;
    font-size: 1rem;
    transition: all 0.4s;
}

.header-bottom-side-left button:hover {
    background-color: darkblue;
}

.header-bottom-side-right {
    flex-basis: 50%;
    display: flex;
    align-items: center;
}

.header-bottom-side-right img {
    width: 115%;
}


@media (min-width: 800px) {
    .navbar {
        position: fixed;  
        top: 0;  
        width: 100%;  
        z-index: 9999;  
    }

    nav ul {
        display: flex;
        justify-content: space-around;  
        width: 100%;  
    }

    .nav-icon-container {
        display: none;
    }

    .nav-menu {
        display: block; 
    }

    .nav-icon-container img:first-child {
        position: fixed;  
        top: 20px;  
        right: 20px;  
        z-index: 1000;  
    }
}


produtos css 

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
  }
  
  .container {
    width: 90%;
    margin: 0 auto;
  }
  
  header {
    text-align: center;
    margin-bottom: 20px;
  }
  
  h1 {
    font-size: 2.5rem;
    color: #333;
  }
  
  .menu {
    display: flex;
    flex-wrap: wrap;
    gap: 20px; /* Espaçamento entre os itens */
    justify-content: space-between;
    padding: 20px;
  }
  
  .item {
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: calc(33% - 20px); /* Faz os itens ocuparem 1/3 da largura do container */
    padding: 15px;
    text-align: center;
    transition: transform 0.3s ease-in-out;
  }
  
  .item img {
    width: 100%;
    max-width: 150px;
    height: auto;
    border-radius: 10px;
    margin-bottom: 10px;
  }
  
  .item h3 {
    font-size: 1.2rem;
    margin-bottom: 10px;
  }
  
  .item p {
    font-size: 1rem;
    color: #666;
    margin-bottom: 10px;
  }
  
  .price {
    font-size: 1.2rem;
    color: #d9534f;
    margin-bottom: 15px;
  }
  
  .add-to-cart {
    background-color: #28a745;
    color: white;
    border: none;
    padding: 10px;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  .add-to-cart:hover {
    background-color: #218838;
  }
  
  footer {
    text-align: center;
    margin-top: 20px;
  }
  
  .view-cart {
    background-color: #007bff;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .view-cart:hover {
    background-color: #0056b3;
  }
  .saiba-mais {
    background-color: #f0ad4e;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
    margin-bottom: 10px; /* Espaço abaixo do botão */
  }
  
  .saiba-mais:hover {
    background-color: #ec971f;
  }
  



