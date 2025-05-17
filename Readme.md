# HabitMaster IGNITE ⚔️ - Forje sua Lenda, um Hábito de Cada Vez!

## 🔥 Sobre o Projeto

HabitMaster IGNITE é um aplicativo interativo e gamificado de construção de hábitos, desenvolvido como projeto para a Imersão IA da Alura. Utilizando o poder da Inteligência Artificial generativa (Google Gemini), este app transforma o processo de desenvolvimento pessoal em uma jornada épica de RPG, onde o usuário é o herói e seus hábitos são as missões a serem conquistadas!

O objetivo é ajudar os usuários a definir, rastrear e manter hábitos positivos de uma forma divertida, motivadora e personalizada, recebendo orientação de um "Mestre de Jogo e Coach de Hábitos" virtual.

**[Link para o vídeo de demonstração (se houver)]** 
**(Adicione o link do seu vídeo aqui quando o tiver)**

**[Link para o projeto no Colab (compartilhável)]** 
**(Compartilhe seu notebook Colab "com qualquer pessoa com o link" e cole o link aqui)**

<!-- 
Substitua o placeholder abaixo por um screenshot real do seu aplicativo em funcionamento!
Para adicionar um screenshot:
1. Tire um print da tela do seu app.
2. Faça upload dessa imagem para a pasta do seu projeto no GitHub.
3. Substitua o link abaixo pelo caminho relativo da imagem no seu repositório. 
   Exemplo: ![Gameplay Screenshot](./screenshots/meu_app.png) 
-->
![App Screenshot](https://via.placeholder.com/700x450.png?text=Insira+um+Screenshot+do+App+HabitMaster+IGNITE+Aqui)

## ✨ Funcionalidades Principais (MVP)

*   **Criação de Jornada Personalizada via Chat com IA:**
    *   O usuário interage com o "HabitMaster IGNITE" (IA) para descrever seus objetivos e aspirações.
    *   A IA faz perguntas de refinamento para entender melhor as necessidades do usuário, tornando o processo guiado.
    *   Com base na conversa, a IA sugere um plano inicial de "Missões" (hábitos) personalizadas.
*   **Plano de Hábitos Gamificado:**
    *   Cada missão/hábito possui:
        *   Um nome temático e divertido.
        *   Uma meta clara e alcançável.
        *   Frequência sugerida (diário, semanal, etc.).
        *   Recompensa em XP (Pontos de Experiência) e Gold (Moedas de Ouro) ao ser concluída.
*   **Dashboard de Missões Interativo (Simulado):**
    *   Visualização clara das missões ativas com seus detalhes.
    *   Sistema de checkboxes (usando `gr.CheckboxGroup`) para o usuário marcar as missões como concluídas dentro da sessão.
*   **Sistema de Progressão Simples:**
    *   Acúmulo de XP e Gold ao completar missões.
    *   Sistema de Níveis: o usuário avança de nível ao atingir marcos de XP.
*   **Interface Amigável e Temática:**
    *   Desenvolvida com Gradio, utilizando uma paleta de cores escura (preto/cinza) com destaques em verde claro, remetendo a um ambiente de jogo e aventura.
*   **Aba "Loja do Aventureiro" (Placeholder):**
    *   Indica planos futuros para utilização do XP e Gold acumulados, como compra de itens virtuais ou customizações, adicionando uma visão de longo prazo para o "jogo".

## 🚀 Tecnologias e Competências Demonstradas

*   **Linguagem de Programação:** Python
*   **Inteligência Artificial Generativa:**
    *   API do Google Gemini (especificamente, o modelo `gemini-1.5-flash-latest` ou similar).
    *   **Engenharia de Prompts Avançada:**
        *   Criação de persona detalhada e consistente para a IA (o "HabitMaster IGNITE").
        *   Desenvolvimento de instruções de sistema (system prompts) complexas para guiar o fluxo conversacional da IA, incluindo a capacidade de fazer perguntas de follow-up e gerar conteúdo estruturado (planos de hábitos em formato Markdown).
        *   Design de prompts para obter respostas formatadas que podem ser parcialmente parseadas pela aplicação.
*   **Interface de Usuário (UI) e Prototipagem Rápida:**
    *   **Gradio:** Utilizado para criar rapidamente uma interface web interativa diretamente do código Python, demonstrando a viabilidade da ideia.
    *   Customização de Temas e CSS Básico: Aplicação de um tema visual coeso (escuro com destaques em verde) para melhorar a experiência do usuário.
    *   Gerenciamento de Estado da UI com `gr.State` para manter a continuidade da sessão do jogo.
*   **Lógica de Aplicação e Gamificação:**
    *   Implementação da lógica de sugestão de hábitos baseada na interação com a IA.
    *   Desenvolvimento de um sistema simples de XP, Gold e Níveis para engajamento do usuário.
    *   Parseamento básico de texto da saída da IA para extrair informações estruturadas (nomes de missão, metas, recompensas).
*   **Manipulação de Dados (em memória):**
    *   Gerenciamento de estado da sessão do usuário (histórico de conversa, plano de hábitos, progresso do jogo) de forma simplificada para o MVP, utilizando variáveis Python.
*   **Ambiente de Desenvolvimento:** Google Colab (Jupyter Notebooks), facilitando a experimentação e o compartilhamento.
*   **Controle de Versão:** Git e GitHub para gerenciamento do código-fonte.

## 🎯 Objetivos do Projeto (Foco na Imersão IA)

*   **Utilidade:** Abordar o desafio comum da formação de hábitos de uma maneira engajadora e personalizada.
*   **Criatividade:** Combinar IA conversacional com mecânicas de gamificação para criar uma experiência de usuário única e motivadora.
*   **Eficácia da IA:** Demonstrar como a IA pode atuar como um coach/mentor interativo, adaptando suas sugestões e planos com base nas entradas do usuário.
*   **Proficiência em Engenharia de Prompts:** O núcleo da inteligência do aplicativo reside na qualidade e detalhamento dos prompts fornecidos ao modelo Gemini, mostrando a capacidade de elicitar comportamentos complexos e respostas estruturadas da IA.

## 🛠️ Como Executar o Projeto (via Google Colab)

1.  **Acesse o Notebook no Google Colab:**
    *   [Link para o Notebook HabitMaster IGNITE](URL_DO_SEU_NOTEBOOK_COMPARTILHADO_AQUI)
    *(Substitua `URL_DO_SEU_NOTEBOOK_COMPARTILHADO_AQUI` pelo link real)*

2.  **Configure sua Chave da API do Google AI:**
    *   Na primeira célula do notebook, você encontrará instruções para configurar sua `GOOGLE_API_KEY_HABITOS`. A forma recomendada é através dos "Secrets" do Colab:
        *   No Colab, clique no ícone de chave (🔑) na barra lateral esquerda.
        *   Adicione um novo secret com o nome `GOOGLE_API_KEY_HABITOS`.
        *   Cole sua chave de API do Google AI Studio (Gemini) no campo "Value".
        *   Certifique-se de que a opção "Notebook access" está marcada.

3.  **Execute as Células em Ordem:**
    *   **Célula 1:** Instalações e Configuração da API Key. Aguarde a conclusão e verifique se a chave da API foi configurada com sucesso.
    *   **Célula 2.1:** Estado da Sessão e Constantes do Sistema.
    *   **Célula 2.2:** Função de Interação com a IA.
    *   **Célula 2.3:** Funções de Gamificação e Parseamento.
    *   **Célula 3 (ou 4, conforme sua última numeração):** Definição e Lançamento da Interface Gradio.
        *   Após a execução desta célula, uma interface Gradio será iniciada e um link público (geralmente com `gradio.live`) será exibido. Clique neste link para abrir o aplicativo em uma nova aba do seu navegador.

4.  **Interaja com o HabitMaster IGNITE!**
    *   Siga as instruções do HabitMaster na interface para definir seus objetivos e receber seu plano de missões gamificado.

## 🔮 Próximos Passos e Melhorias Futuras (Pós-Imersão)

*   **Persistência de Dados:** Implementar um sistema de banco de dados (ex: SQLite, Firebase) para salvar o progresso do usuário, hábitos e configurações entre sessões, junto com um sistema de login/autenticação.
*   **Interatividade Avançada no Dashboard:** Permitir que os checkboxes de conclusão de hábitos sejam diretamente clicáveis e atualizem o estado sem depender apenas do input de texto para a IA.
*   **Desenvolvimento da Loja:** Implementar a funcionalidade da "Loja do Aventureiro" onde XP e Gold podem ser usados.
*   **Sistema de Recompensas e Conquistas:** Expandir a gamificação com badges, conquistas e recompensas mais variadas.
*   **Lembretes e Notificações:** Integrar um sistema para lembrar o usuário de seus hábitos.
*   **Análise de Progresso e Feedback Contínuo da IA:** A IA poderia analisar o progresso ao longo do tempo e oferecer novas sugestões ou ajustes nas missões.
*   **Melhoria no Parseamento da IA:** Explorar o retorno de JSON pela IA para um parseamento de dados mais robusto e menos dependente da formatação exata do Markdown.

## 🤝 Contribuições

Este projeto foi desenvolvido como parte da Imersão IA da Alura. Feedback e sugestões são bem-vindos!

*Desenvolvido com 🧠 e 🔥 por João Batista Ribeiro Neto *
