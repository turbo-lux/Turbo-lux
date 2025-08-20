<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CRESCIMENTO TÁTICO - Sua Estratégia de Autoridade</title>
    <style>
        :root {
            --color-primary: #25D366; /* Verde WhatsApp */
            --color-dark: #121212;
            --color-light: #F5F5F5;
            --color-accent: #FF9900;
            --color-gray: #333;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--color-dark);
            color: var(--color-light);
            line-height: 1.6;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        header {
            text-align: center;
            padding: 2rem 0;
            border-bottom: 1px solid var(--color-gray);
        }
        h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--color-primary);
        }
        .subheadline {
            font-size: 1.2rem;
            color: #ccc;
        }
        .trust-badges {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 2rem 0;
            flex-wrap: wrap;
        }
        .badge {
            text-align: center;
            background: var(--color-gray);
            padding: 10px 15px;
            border-radius: 5px;
            font-size: 0.9rem;
        }
        .badge i { /* Ícone simbólico */
            font-size: 1.5rem;
            margin-bottom: 5px;
            color: var(--color-accent);
        }
        .video-container {
            background: #000;
            padding: 20px;
            border-radius: 10px;
            margin: 2rem 0;
            text-align: center;
        }
        .video-placeholder {
            background: #222;
            height: 250px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #999;
            border-radius: 5px;
        }
        .pricing {
            background: var(--color-gray);
            padding: 2rem;
            border-radius: 10px;
            margin: 2rem 0;
        }
        .plans-comparison {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 15px;
            margin-top: 1rem;
        }
        .plan {
            background: #222;
            padding: 1.5rem;
            border-radius: 5px;
            text-align: center;
            border: 2px solid transparent;
        }
        .plan.popular {
            border-color: var(--color-accent);
            transform: scale(1.05);
            position: relative;
        }
        .plan.popular::before {
            content: "MAIS ESCOLHIDO";
            position: absolute;
            top: -12px;
            left: 50%;
            transform: translateX(-50%);
            background: var(--color-accent);
            color: black;
            font-weight: bold;
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 0.7rem;
        }
        .plan-name {
            font-size: 1.2rem;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .plan-price {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--color-primary);
            margin-bottom: 15px;
        }
        .plan-features {
            list-style: none;
            padding: 0;
            margin: 0 0 20px 0;
            font-size: 0.9rem;
        }
        .plan-features li {
            margin-bottom: 8px;
            padding-left: 20px;
            position: relative;
        }
        .plan-features li::before {
            content: "✔️";
            position: absolute;
            left: 0;
        }
        .plan-features li.cross::before {
            content: "❌";
        }
        .btn {
            display: inline-block;
            padding: 15px 30px;
            background: var(--color-primary);
            color: black !important;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            border: none;
            cursor: pointer;
            width: 100%;
            text-align: center;
            transition: background 0.3s;
        }
        .btn:hover {
            background: #1da851;
        }
        .guarantee {
            text-align: center;
            margin: 2rem 0;
            font-style: italic;
            color: #ccc;
        }
        .faq {
            margin: 3rem 0;
        }
        .faq-item {
            margin-bottom: 15px;
            border-bottom: 1px solid var(--color-gray);
            padding-bottom: 15px;
        }
        .faq-question {
            font-weight: bold;
            cursor: pointer;
        }
        .faq-answer {
            display: none;
            margin-top: 10px;
            padding-left: 15px;
            color: #ccc;
        }
        .faq-answer.active {
            display: block;
        }
        .urgency {
            text-align: center;
            background: var(--color-accent);
            color: black;
            padding: 10px;
            border-radius: 5px;
            margin: 2rem 0;
            font-weight: bold;
        }
        footer {
            text-align: center;
            padding: 2rem 0;
            border-top: 1px solid var(--color-gray);
            font-size: 0.8rem;
            color: #999;
        }
        /* Estilos para o modal de checkout */
        .checkout-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            z-index: 1000;
            align-items: center;
            justify-content: center;
        }
        .checkout-content {
            background: var(--color-dark);
            padding: 2rem;
            border-radius: 10px;
            width: 90%;
            max-width: 500px;
            border: 2px solid var(--color-primary);
        }
        .close-modal {
            float: right;
            cursor: pointer;
            font-size: 1.5rem;
        }
    </style>
</head>
<body>

    <div class="container">

        <header>
            <h1>CRESCIMENTO TÁTICO</h1>
            <p class="subheadline">Não é mágica. É estratégia. Construa autoridade real sem gastar fortunas em bots que caem.</p>
        </header>

        <div class="trust-badges">
            <div class="badge">
                <div>🔒</div>
                NF-e & Pix Rastreável
            </div>
            <div class="badge">
                <div>🔄</div>
                Reposição Garantida
            </div>
            <div class="badge">
                <div>📊</div>
                Dados Transparentes
            </div>
        </div>

        <div class="video-container">
            <div class="video-placeholder">
                <!-- Substitua por um vídeo real do Vimeo/YouTube -->
                [VÍDEO EXPLICATIVO: Como a estratégia de crescimento tático funciona]
            </div>
        </div>

        <div class="pricing">
            <h2 style="text-align: center;">ESCOLHA SEU NIVEL DE COMPROMISSO</h2>
            <p style="text-align: center; color: #ccc;">Seja esperto. Comece com o tático, escale para o premium.</p>

            <div class="plans-comparison">
                <!-- Plano Econômico -->
                <div class="plan">
                    <div class="plan-name">ECONÔMICO</div>
                    <div class="plan-price">R$ 97</div>
                    <ul class="plan-features">
                        <li>500 Seguidores</li>
                        <li>Rede de Entrada</li>
                        <li><strong>Queda estimada: ~30%</strong></li>
                        <li>Reposição em 15 dias</li>
                        <li class="cross">Suporte Prioritário</li>
                        <li class="cross">Relatório de Crescimento</li>
                    </ul>
                    <a href="#" class="btn" onclick="openCheckout('Econômico', 97)">SELECIONAR</a>
                </div>

                <!-- Plano Intermediário (DESTAQUE) -->
                <div class="plan popular">
                    <div class="plan-name">INTERMEDIÁRIO</div>
                    <div class="plan-price">R$ 247</div>
                    <ul class="plan-features">
                        <li>1.500 Seguidores</li>
                        <li>Rede Sólida</li>
                        <li><strong>Queda quase zero em 30d</strong></li>
                        <li>Reposição em 30 dias</li>
                        <li>Suporte 72h</li>
                        <li class="cross">Relatório de Crescimento</li>
                    </ul>
                    <a href="#" class="btn" onclick="openCheckout('Intermediário', 247)">SELECIONAR</a>
                </div>

                <!-- Plano Premium -->
                <div class="plan">
                    <div class="plan-name">PREMIUM</div>
                    <div class="plan-price">R$ 497</div>
                    <ul class="plan-features">
                        <li>3.500 Seguidores</li>
                        <li>Rede Blindada</li>
                        <li><strong>Permanência 99%+</strong></li>
                        <li>Reposição Vitalícia</li>
                        <li>Suporte 24/7</li>
                        <li>Relatório de Crescimento</li>
                    </ul>
                    <a href="#" class="btn" onclick="openCheckout('Premium', 497)">SELECIONAR</a>
                </div>
            </div>
        </div>

        <div class="urgency">
            ⚠️ OFERTA POR TEMPO LIMITADO: Garanta o preço de lançamento! Preço sobe após as primeiras 50 vendas.
        </div>

        <div class="guarantee">
            ✅ COMPRA 100% SEGURA: 7 DIAS DE GARANTIA. Se não ficar satisfeito, devolvemos seu dinheiro. Sem perguntas.
        </div>

        <div class="faq">
            <h2>PERGUNTAS FREQUENTES</h2>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">+ Isso não é golpe?</div>
                <div class="faq-answer">Golpe é prometer o que não entrega. Aqui mostramos tudo: a queda possível, os prazos, a reposição. Trabalhamos com nota fiscal e transparência total. Você está comprando uma ferramenta, não um milagre.</div>
            </div>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">+ Como é a reposição?</div>
                <div class="faq-answer">Simples: acompanhamos sua conta. Se dentro do prazo de garantia do seu plano (15 ou 30 dias) houver uma queda anormal, repomos automaticamente. Basta nos enviar um print.</div>
            </div>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">+ Meu perfil pode ser bloqueado?</div>
                <div class="faq-answer">O risco existe em qualquer plataforma, mas é mínimo (menos de 0.5% dos casos). Usamos métodos de entrega orgânicos para minimizar ao máximo qualquer chance de bloqueio.</div>
            </div>
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">+ Como recebo os seguidores?</div>
                <div class="faq-answer">A entrega é inicializada em até 24h após a confirmação do pagamento. A velocidade é gradual para parecer o mais natural possível e pode levar de 2 a 5 dias para completar.</div>
            </div>
        </div>

        <footer>
            © 2023 Crescimento Tático. Este serviço não é endossado ou certificado pelo Instagram/Meta. Todos os direitos reservados.
        </footer>
    </div>

    <!-- Modal de Checkout -->
    <div class="checkout-modal" id="checkoutModal">
        <div class="checkout-content">
            <span class="close-modal" onclick="closeCheckout()">&times;</span>
            <h2>Finalizar Compra: <span id="selectedPlan">Plano</span></h2>
            <p>Valor: <strong id="planPrice">R$ 0</strong></p>
            <p>Preencha os dados abaixo para gerar o Pix e a Nota Fiscal.</p>
            <form id="checkoutForm">
                <input type="text" placeholder="Nome Completo" required style="width: 100%; padding: 10px; margin: 10px 0; box-sizing: border-box; background: #222; color: white; border: 1px solid #444;">
                <input type="email" placeholder="E-mail" required style="width: 100%; padding: 10px; margin: 10px 0; box-sizing: border-box; background: #222; color: white; border: 1px solid #444;">
                <input type="text" placeholder="@seuusuario" required style="width: 100%; padding: 10px; margin: 10px 0; box-sizing: border-box; background: #222; color: white; border: 1px solid #444;">
                <button type="submit" class="btn">GERAR PIX E NF-E</button>
            </form>
        </div>
    </div>

    <script>
        function toggleFaq(element) {
            const answer = element.nextElementSibling;
            answer.classList.toggle('active');
        }

        function openCheckout(planName, planPrice) {
            document.getElementById('selectedPlan').textContent = planName;
            document.getElementById('planPrice').textContent = 'R$ ' + planPrice;
            document.getElementById('checkoutModal').style.display = 'flex';
        }

        function closeCheckout() {
            document.getElementById('checkoutModal').style.display = 'none';
        }

        document.getElementById('checkoutForm').addEventListener('submit', function(e) {
            e.preventDefault();
            // Aqui você integraria com uma API de pagamento (ex: Mercado Pago, ASAAS)
            alert('Em um sistema real, isso geraria o PIX e a NF-e. Redirecionando para o WhatsApp...');
            // window.location.href = 'https://wa.me/5511999999999?text=Comprei%20o%20plano%20[PLANO]';
        });

        // Fecha o modal clicando fora dele
        window.onclick = function(event) {
            const modal = document.getElementById('checkoutModal');
            if (event.target == modal) {
                closeCheckout();
            }
        }
    </script>

</body>
</html>
