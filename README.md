# Anam Med English

Plataforma de triagem e validação de proficiência em inglês para médicos e profissionais da saúde que desejam atuar no atendimento a pacientes reais.

## 📌 Sobre o Projeto

O **Anam Med English** é uma aplicação web que utiliza avatares interativos de Inteligência Artificial (Anam AI) para simular consultas médicas reais em inglês. O objetivo é avaliar, de forma automatizada e segura, a capacidade de comunicação do profissional de saúde antes de sua entrada no mercado internacional.

A plataforma captura a fala do médico durante a simulação, processa as transcrições em tempo real e gera um relatório detalhado com base em métricas linguísticas.

## ⚙️ Como Funciona

1. **Simulação:** O médico interage com um paciente virtual (avatar) em inglês através do widget da Anam AI.
2. **Captura:** O sistema escuta e captura as transcrições da conversa via eventos do widget.
3. **Avaliação:** A plataforma calcula o score com base em cinco pilares:
   - Tempo de fala;
   - Quantidade de palavras ditas;
   - Tamanho médio das frases;
   - Diversidade de vocabulário;
   - Uso de palavras-chave do contexto médico.
4. **Classificação:** O resultado é mapeado para o Quadro Europeu Comum de Referência (CEFR), indo de **A1** (Iniciante) a **C2** (Proficiente).
5. **Aprovação:** Para ser aprovado e aguardar a publicação do perfil, o médico precisa atingir no mínimo o nível **B2** (Intermediário Alto).

## 🛡️ Regras de Segurança

Para garantir a integridade das avaliações e a segurança do sistema, foram implementadas as seguintes regras:
- O candidato possui no máximo **2 tentativas** de avaliação.
- Caso seja reprovado na segunda tentativa, seu endereço de IP é **bloqueado por 72 horas**.
- O controle de tentativas e bloqueios é gerenciado localmente (`localStorage`) para persistência durante o acesso.

## 🛠️ Tecnologias Utilizadas

- **HTML5 / CSS3 / JavaScript** (Vanilla)
- **Anam AI** (Widget de Avatar e Eventos de Sincronização)
- **LocalStorage / SessionStorage** (Controle de estado e tentativas)

## 📂 Estrutura do Repositório

anam-med-english/
├── index.html                       # Tela de consulta e simulação com o avatar
├── relatorio.html                   # Tela de processamento e exibição do relatório
├── obrigado.html                    # Tela de sucesso após aprovação
├── ESTRUTURA.txt                    # Documentação interna do projeto
├── eventosquedaparacontrolar.txt    # Anotações sobre eventos do widget
├── README.md                        # Documentação principal do repositório
└── LICENSE                          # Licença de uso

## 🚀 Como Executar

1. Clone este repositório:
   git clone https://github.com/seu-usuario/anam-med-english.git
2. Abra o arquivo `index.html` em qualquer navegador moderno.
3. Permita o acesso ao microfone e inicie a consulta.

---
*Desenvolvido para garantir que a barreira do idioma não comprometa a segurança e a qualidade do atendimento clínico.*
