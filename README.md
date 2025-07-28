CBT Bot — Chatbot de Terapia Cognitivo-Comportamental com LLMs
📋 Descrição do Projeto
Este projeto desenvolve um chatbot terapêutico automatizado (CBT Bot) utilizando Modelos de Linguagem de Grande Porte (LLMs) da OpenAI para auxiliar usuários a lidarem com emoções e pensamentos negativos com base em princípios da Terapia Cognitivo-Comportamental (TCC).

O chatbot é treinado e testado utilizando a base de dados pública do Kaggle Human and LLM Mental Health Conversations, que contém diálogos reais e gerados por LLMs sobre saúde mental.

🎯 Objetivo
Criar um assistente virtual empático que:

- Identifique distorções cognitivas comuns nos textos do usuário;

- Responda com mensagens baseadas em regras da TCC para reestruturar pensamentos negativos;

- Use LLMs da OpenAI para gerar respostas mais naturais e variadas quando o padrão de distorção não for detectado;

- Permita um atendimento automatizado inicial para pessoas que buscam apoio emocional.

  🧩 Estrutura do Projeto
- dataset.csv: base de dados original do Kaggle com diálogos de saúde mental.
- Script para converter o CSV em JSONL, formato compatível com fine-tuning OpenAI.
- Implementação do chatbot com:
- Detecção de distorções cognitivas via regras;
- Respostas baseadas nessas regras (TCC Bot);
- Fallback para respostas geradas pela API OpenAI GPT-4o-mini;
- Função para manter histórico de interações;
- Visualizações exploratórias (gráficos de frequência, polaridade, tamanho das mensagens);
- Código para interagir com o chatbot via terminal.


🛠 Tecnologias e Bibliotecas Utilizadas
- Python 3.x
- Pandas (manipulação de dados)
- Matplotlib (visualização de dados)
- TextBlob (análise de sentimento)
- OpenAI Python SDK (integração com API GPT-4o-mini)
- Regex (para detecção de distorções cognitivas)

  🚀 Como Rodar
Clone este repositório ou baixe os arquivos.
Instale as dependências:
pip install pandas matplotlib textblob openai
Configure sua chave de API OpenAI em uma variável de ambiente chamada OPENAI_API_KEY ou defina diretamente no código.

Execute o chatbot:
python cbt_bot.py
Digite suas mensagens e interaja com o bot. Para sair, digite sair.

📊 Análise Exploratória dos Dados
- Distribuição do tamanho das mensagens dos usuários;
- Frequência das distorções cognitivas detectadas no histórico;
- Polaridade dos textos para analisar sentimentos;
- Visualizações para compreensão da base de dados e comportamento do bot.

💡 Resultados e Conclusão
O chatbot combina regras baseadas em TCC com respostas geradas por LLMs para maior naturalidade e efetividade.
- A base do Kaggle possibilitou um conjunto realista para treinamento e validação.
- Ferramentas analíticas mostraram padrões úteis para entender as emoções dos usuários.
- O sistema oferece um suporte inicial útil, podendo ser expandido para incluir integração com profissionais da saúde.

⚠️ Limitações
- O chatbot não substitui acompanhamento psicológico profissional.
- Possui respostas limitadas às regras programadas e qualidade das respostas da API.
- Requer conexão e créditos válidos para uso da API OpenAI.



📚 Referências
- Base de dados Kaggle - Human and LLM Mental Health Conversations
- OpenAI API Documentation
- Beck, A. T. (1976). Cognitive Therapy and the Emotional Disorders.


  
