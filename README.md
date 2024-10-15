<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emilly Borges Advocacia</title>
    <style>
        /* CSS interno */
        @import url('https://fonts.googleapis.com/css2?family=Garamond&display=swap'); /* Importando a fonte Garamond */

        body, html {
            margin: 0;
            padding: 0;
            font-family: 'Garamond', serif; /* Alterando a fonte para Garamond */
            background-color: #f4f4f4; /* Fundo mais suave */
            color: #333; /* Texto em uma cor mais escura */
        }

        header {
            background: linear-gradient(to right, #1a1a1a, #333); /* Gradiente de fundo para um visual moderno */
            padding: 15px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            display: flex;
            flex-direction: column; /* Alinha itens em coluna */
            align-items: center; /* Centraliza itens */
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5); /* Sombra mais forte */
        }

        header .container {
            display: flex;
            flex-direction: column; /* Alinha logo e menu em coluna */
            align-items: center; /* Centraliza logo e menu */
            width: 90%;
            margin: auto;
        }

        h1 {
            color: #f0f0f0; /* Cor do título */
            font-size: 2.5em; /* Tamanho maior do h1 */
            text-align: center; /* Centraliza o título */
            margin-bottom: 10px; /* Espaço abaixo do título */
        }

        nav ul {
            list-style: none;
            display: flex;
            margin: 0;
            padding: 0;
            justify-content: center; /* Centraliza itens do menu */
            flex-wrap: wrap; /* Permite que os itens do menu quebrem para a próxima linha em telas menores */
        }

        nav ul li {
            margin: 0 10px; /* Espaçamento horizontal entre os itens */
        }

        nav ul li a {
            color: #f0f0f0; /* Cor do texto do link */
            text-decoration: none; /* Remove o sublinhado */
            padding: 10px 15px; /* Espaçamento interno */
            transition: background 0.3s, color 0.3s, transform 0.3s; /* Transição suave */
            border-radius: 5px; /* Bordas arredondadas nos links */
        }

        nav ul li a:hover {
            background-color: #007bff; /* Azul ao passar o mouse */
            color: #fff; /* Texto branco ao passar o mouse */
            transform: scale(1.05); /* Efeito de zoom */
        }

        .hero {
            background: url('images/banner.jpg') center/cover no-repeat;
            color: #fff;
            height: 70vh; /* Ajustado para uma altura menor */
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            flex-direction: column; /* Centraliza a logo e o texto */
            filter: brightness(0.7); /* Escurece o fundo da hero para melhor contraste */
        }

        .hero img {
            width: 80%; /* Reduzido para ser responsivo */
            max-width: 500px; /* Largura máxima */
            height: auto; /* Mantém a proporção */
            margin-bottom: 20px; /* Espaçamento entre a logo e o texto */
        }

        .hero h1 {
            font-size: 2.5em; /* Tamanho menor do h1 */
            margin-bottom: 10px;
        }

        .section {
            padding: 40px 20px; /* Ajustado para ser mais responsivo */
            background-color: #fff; /* Fundo branco para as seções */
            text-align: center;
        }

        .section h2 {
            margin-bottom: 20px;
            color: #000;
            font-size: 2.5em; /* Tamanho maior do h2 */
        }

        .section p, .section ul {
            max-width: 800px;
            margin: auto;
            color: #666;
            font-size: 1.2em; /* Tamanho de fonte um pouco maior */
        }

        .servicos-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px; /* Espaçamento entre os ícones */
}

.servico {
    background-color: #e0e0e0; /* Cor de fundo dos serviços */
    border-radius: 8px;
    padding: 20px;
    width: 220px; /* Largura do bloco de serviço */
    text-align: center;
    color: #000;
    transition: transform 0.3s; /* Transição suave */
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Sombra para dar profundidade */
}

.servico:hover {
    transform: scale(1.05); /* Efeito de zoom ao passar o mouse */
}

.servico-link {
    color: inherit; /* Herda a cor do texto */
    text-decoration: none; /* Remove o sublinhado */
    display: block; /* Para que o link ocupe todo o espaço */
    height: 100%; /* Para que o link ocupe toda a altura do serviço */
}

        .botao-servico {
    display: inline-block;
    background-color: #808080; 
    color: #fff;
    padding: 15px;
    border-radius: 8px; /* Bordas arredondadas */
    text-decoration: none; /* Remove o sublinhado */
    transition: background-color 0.3s, transform 0.3s;
    margin-top: 10px; /* Espaçamento entre os botões */
}

.botao-servico:hover {
    background-color: #808080; 
    transform: scale(1.05); /* Efeito de zoom ao passar o mouse */
}

        footer {
            background-color: #000;
            color: #f0f0f0;
            text-align: center;
            padding: 15px 0;
        }

        footer a {
            color: #f0f0f0;
            text-decoration: none;
        }

        /* Estilo específico para os textos explicativos */
        .descricao {
            color: #666;
            font-size: 1em; /* Tamanho de fonte menor para descrições */
            margin-top: 5px; /* Espaçamento acima das descrições */
        }

        /* Media Queries para responsividade */
        @media (max-width: 300px) {
            .hero {
                height: 50vh; /* Altura ajustada para telas menores */
            }

            .hero h1 {
                font-size: 2em; /* Tamanho menor do h1 para telas menores */
            }

            .section h2 {
                font-size: 2em; /* Tamanho menor do h2 */
            }

            .servico {
                width: 90%; /* Largura maior em telas menores */
            }

            nav ul li {
                margin: 0 5px; /* Reduzir espaçamento em telas menores */
            }
        }

        @media (max-width: 100px) {
            .hero h1 {
                font-size: 1.5em; /* Tamanho ainda menor do h1 para telas muito pequenas */
            }

            .section p {
                font-size: 1em; /* Tamanho de fonte menor para descrições */
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Emilly Borges Advocacia</h1>
            <nav>
                <ul>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#servicos">Serviços</a></li>
                    <li><a href="#compromisso">Compromisso</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <img src="c:\Users\paula\OneDrive\Imagens\LogoFinal.png" alt="Logo Emilly Borges Advocacia"> <!-- Logo inserida aqui -->
        <div>
            <h1>Compromisso com a Justiça e Ética Profissional</h1> <!-- Texto do h1 atualizado -->
        </div>
    </section>

    <section id="sobre" class="section">
        <h2>Sobre Nós</h2>
        <p style="font-size: 1.3em;">Emilly Borges Advocacia é um escritório especializado em oferecer soluções jurídicas de alta qualidade, focado em resultados e na melhor defesa dos interesses dos nossos clientes.</p>
    </section>

    <section id="contato" class="section">
        <h2>Entre em Contato</h2>
        <a href="https://wa.me/5543998061335?text=Gostaria%20de%20saber%20mais" class="botao-servico">Entre em Contato</a>
    </section>

   <section id="servicos" class="section">
    <h2>Nossos Serviços</h2>
    <div class="servicos-container">
        <div class="servico">
            <a href="https://wa.me/5543998061335?text=Gostaria de saber mais sobre Direito Civil." target="_blank" class="servico-link">
                <h3>Direito Civil</h3>
                <p class="descricao">Assessoria em questões de natureza civil, incluindo contratos, obrigações e responsabilidade civil.</p>
            </a>
        </div>
        <div class="servico">
            <a href="https://wa.me/5543998061335?text=Gostaria de saber mais sobre Direito Trabalhista." target="_blank" class="servico-link">
                <h3>Direito Trabalhista</h3>
                <p class="descricao">Consultoria e representação em demandas trabalhistas, visando proteger os direitos dos trabalhadores e empregadores.</p>
            </a>
        </div>
        <div class="servico">
            <a href="https://wa.me/5543998061335?text=Gostaria de saber mais sobre Direito Empresarial." target="_blank" class="servico-link">
                <h3>Direito Empresarial</h3>
                <p class="descricao">Apoio jurídico em questões empresariais, como constituição de empresas, contratos e litígios.</p>
            </a>
        </div>
        <div class="servico">
            <a href="https://wa.me/5543998061335?text=Gostaria de saber mais sobre Consultoria Jurídica." target="_blank" class="servico-link">
                <h3>Consultoria Jurídica</h3>
                <p class="descricao">Orientação e análise de situações jurídicas para uma melhor tomada de decisão.</p>
            </a>
        </div>
    </div>
</section>

    
    

    <section id="compromisso" class="section">
        <h2>Compromisso e Integridade</h2>
        <p>Entenda como será seu atendimento:</p>
        <p>Nossos profissionais estão preparados para oferecer um atendimento próximo, respeitoso e com total transparência em todas as etapas do processo.</p>
        <div class="servicos-container">
            <div class="servico">
                <h3>Atendimento Humanizado</h3>
                <p class="descricao">Focamos em entender suas necessidades e oferecer soluções personalizadas.</p>
            </div>
            <div class="servico">
                <h3>Transparência Total</h3>
                <p class="descricao">Mantemos você informado sobre cada etapa do seu caso.</p>
            </div>
            <div class="servico">
                <h3>Ética Profissional</h3>
                <p class="descricao">Atuamos sempre com base em princípios éticos, defendendo seus interesses com responsabilidade.</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2023 Advocacia Emilly Borges - Todos os direitos reservados.   /* CSS interno */
            @import url('https://fonts.googleapis.com/css2?family=Garamond&display=swap'); /* Importando a fonte Garamond */
    
            body, html {
                margin: 0;
                padding: 0;
                font-family: 'Garamond', serif; /* Alterando a fonte para Garamond */
                background-color: #f4f4f4; /* Fundo mais suave */
                color: #333; /* Texto em uma cor mais escura */
            }
    
            header {
                background: linear-gradient(to right, #1a1a1a, #333); /* Gradiente de fundo para um visual moderno */
                padding: 15px 0;
                position: fixed;
                width: 100%;
                top: 0;
                z-index: 1000;
                display: flex;
                flex-direction: column; /* Alinha itens em coluna */
                align-items: center; /* Centraliza itens */
                box-shadow: 0 2px 10px rgba(0, 0, 0, 0.5); /* Sombra mais forte */
            }
    
            header .container {
                display: flex;
                flex-direction: column; /* Alinha logo e menu em coluna */
                align-items: center; /* Centraliza logo e menu */
                width: 90%;
                margin: auto;
            }
    
            h1 {
                color: #f0f0f0; /* Cor do título */
                font-size: 2.5em; /* Tamanho maior do h1 */
                text-align: center; /* Centraliza o título */
                margin-bottom: 10px; /* Espaço abaixo do título */
            }
    
            nav ul {
                list-style: none;
                display: flex;
                margin: 0;
                padding: 0;
                justify-content: center; /* Centraliza itens do menu */
                flex-wrap: wrap; /* Permite que os itens do menu quebrem para a próxima linha em telas menores */
            }
    
            nav ul li {
                margin: 0 10px; /* Espaçamento horizontal entre os itens */
            }
    
            nav ul li a {
                color: #f0f0f0; /* Cor do texto do link */
                text-decoration: none; /* Remove o sublinhado */
                padding: 10px 15px; /* Espaçamento interno */
                transition: background 0.3s, color 0.3s, transform 0.3s; /* Transição suave */
                border-radius: 5px; /* Bordas arredondadas nos links */
            }
    
            nav ul li a:hover {
                background-color: #007bff; /* Azul ao passar o mouse */
                color: #fff; /* Texto branco ao passar o mouse */
                transform: scale(1.05); /* Efeito de zoom */
            }
    
            .hero {
                background: url('images/banner.jpg') center/cover no-repeat;
                color: #fff;
                height: 70vh; /* Ajustado para uma altura menor */
                display: flex;
                justify-content: center;
                align-items: center;
                text-align: center;
                flex-direction: column; /* Centraliza a logo e o texto */
                filter: brightness(0.7); /* Escurece o fundo da hero para melhor contraste */
            }
    
            .hero img {
                width: 80%; /* Reduzido para ser responsivo */
                max-width: 500px; /* Largura máxima */
                height: auto; /* Mantém a proporção */
                margin-bottom: 20px; /* Espaçamento entre a logo e o texto */
            }
    
            .hero h1 {
                font-size: 2.5em; /* Tamanho menor do h1 */
                margin-bottom: 10px;
            }
    
            .section {
                padding: 40px 20px; /* Ajustado para ser mais responsivo */
                background-color: #fff; /* Fundo branco para as seções */
                text-align: center;
            }
    
            .section h2 {
                margin-bottom: 20px;
                color: #000;
                font-size: 2.5em; /* Tamanho maior do h2 */
            }
    
            .section p, .section ul {
                max-width: 800px;
                margin: auto;
                color: #666;
                font-size: 1.2em; /* Tamanho de fonte um pouco maior */
            }
    
            .servicos-container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 20px; /* Espaçamento entre os ícones */
    }
    
    .servico {
        background-color: #e0e0e0; /* Cor de fundo dos serviços */
        border-radius: 8px;
        padding: 20px;
        width: 220px; /* Largura do bloco de serviço */
        text-align: center;
        color: #000;
        transition: transform 0.3s; /* Transição suave */
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Sombra para dar profundidade */
    }
    
    .servico:hover {
        transform: scale(1.05); /* Efeito de zoom ao passar o mouse */
    }
    
    .servico-link {
        color: inherit; /* Herda a cor do texto */
        text-decoration: none; /* Remove o sublinhado */
        display: block; /* Para que o link ocupe todo o espaço */
        height: 100%; /* Para que o link ocupe toda a altura do serviço */
    }
    
            .botao-servico {
        display: inline-block;
        background-color: #808080; 
        color: #fff;
        padding: 15px;
        border-radius: 8px; /* Bordas arredondadas */
        text-decoration: none; /* Remove o sublinhado */
        transition: background-color 0.3s, transform 0.3s;
        margin-top: 10px; /* Espaçamento entre os botões */
    }
    
    .botao-servico:hover {
        background-color: #808080; 
        transform: scale(1.05); /* Efeito de zoom ao passar o mouse */
    }
    
            footer {
                background-color: #000;
                color: #f0f0f0;
                text-align: center;
                padding: 15px 0;
            }
    
            footer a {
                color: #f0f0f0;
                text-decoration: none;
            }
    
            /* Estilo específico para os textos explicativos */
            .descricao {
                color: #666;
                font-size: 1em; /* Tamanho de fonte menor para descrições */
                margin-top: 5px; /* Espaçamento acima das descrições */
            }
    
            /* Media Queries para responsividade */
            @media (max-width: 300px) {
                .hero {
                    height: 50vh; /* Altura ajustada para telas menores */
                }
    
                .hero h1 {
                    font-size: 2em; /* Tamanho menor do h1 para telas menores */
                }
    
                .section h2 {
                    font-size: 2em; /* Tamanho menor do h2 */
                }
    
                .servico {
                    width: 90%; /* Largura maior em telas menores */
                }
    
                nav ul li {
                    margin: 0 5px; /* Reduzir espaçamento em telas menores */
                }
            }
    
            @media (max-width: 100px) {
                .hero h1 {
                    font-size: 1.5em; /* Tamanho ainda menor do h1 para telas muito pequenas */
                }
    
                .section p {
                    font-size: 1em; /* Tamanho de fonte menor para descrições */
                }
            } </p>
        <p>Feito por <a href="https://www.linkedin.com/in/paula-beltrami-303211290/" target="_blank">Paula Beltrami</a></p>
    </footer>
</body>
</html>
