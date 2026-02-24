# 💸 App de Organização de Finanças Pessoais com Vibe Coding

**PRD Refinado no Gemini:**

```Prompt
Aja como um desenvolvedor Full Stack Sênior e arquiteto de software. Crie um Web App de Finanças Pessoais Conversacional chamado VibeFinance utilizando React, Tailwind CSS, Shadcn/UI e Firebase.

1. Configuração do Firebase:

Autenticação: Implemente login via Google e E-mail (Firebase Auth). O app deve ter uma 'Landing Page' de boas-vindas para usuários deslogados.

Firestore: Crie uma coleção transactions vinculada ao uid do usuário. Campos: description (string), amount (number), category (string), type (income/expense), e createdAt (timestamp).

Persistência: Garanta que os dados sejam lidos e gravados em tempo real no Firestore.

2. Interface 'Zero UI' (Chat-First):

Layout mobile-first com abas inferiores: 💬 Chat, 📊 Dashboard e 🎯 Metas.

Mensagem de Boas-Vindas: Ao logar pela primeira vez, o Agente deve dizer: 'Olá! Sou seu assistente do VibeFinance. 🚀 Guardar dinheiro não precisa ser chato. Sempre que gastar ou receber algo, é só me contar aqui. Ex: "Gastei 30 no Uber" ou "Recebi 5000 de salário". Por onde quer começar?'

3. Engine de Processamento de Linguagem (NLP Simulado):
Desenvolva uma função que processe a entrada do usuário e classifique automaticamente usando este dicionário:

Essenciais: Aluguel, Condomínio, Luz, Água, Internet, Mercado, Feira.

Alimentação: Restaurante, Ifood, Pizza, Lanche, Almoço, Café, Padaria.

Transporte: Uber, 99, Gasolina, Combustível, Ônibus, Metrô.

Lazer: Cinema, Show, Bar, Cerveja, Netflix, Spotify, Viagem.

Saúde: Farmácia, Remédio, Médico, Academia.

Entradas: Salário, Bônus, Pix, Recebi, Pagamento, Freelance.
Lógica: Identifique o valor numérico na frase. Se não houver categoria clara, salve como 'Outros' e peça confirmação.

4. Dashboard e Inteligência do Agente:

Visão de Sobrevivência: No Dashboard, exiba o 'Saldo Livre' (Receitas - Despesas Essenciais).

Gráficos: Use Recharts para um gráfico de pizza por categoria e um gráfico de barras comparando Entradas vs Saídas.

Alertas Proativos: Se o gasto total de uma categoria exceder 70% da média mensal, o Agente deve enviar uma mensagem de alerta no chat: '⚠️ Opa! Seus gastos com [Categoria] estão acima do normal hoje. Vamos dar uma segurada?'

5. Estética e UX:

Estilo 'Minimalista Moderno' com bordas arredondadas e sombras suaves.

Use ícones da Lucide-React.

Use tons de verde para ganhos e tons de coral/vermelho para gastos.

Implemente 'Toasts' para confirmar cada transação salva com sucesso."
```

**Interações com a IA (Firebase Studio) e configurações principais:**
- Necessário configurar uma chave API para vínculo com o sistema de autenticação, esta chave pode ser gerada no console do Google Cloud. Após gerada e confirgurada, informei através do console da própria IA do Firebase Studio (Não compartilhe sua chave API com ninguém).
- Para a tela de login, foi necessário criar uma condição do Firebase Console, em Criação>Authentication>Método de Login: E-mail/senha e Google - Habilitadas essas duas chaves, o sistema já estava pronto para uso. Ou então solicitar a criação de usuário teste.
- Necessário ativar API Gemini no Google Cloud para a interpretação de linguagem natural.

**Resumo sobre o que o App de finanças faz:**

🚀 VibeFinance: O Fim das Planilhas Chatas
O VibeFinance é um assistente pessoal de finanças que transforma a gestão do dinheiro em uma conversa casual. Em vez de formulários complexos e tabelas infinitas, o usuário organiza sua vida financeira apenas conversando.

🧠 O Conceito: "Zero UI"
Acreditamos que o melhor app de finanças é aquele que não parece um app de finanças. O foco total está na linguagem natural: você fala como se estivesse mandando um zap para um amigo, e a inteligência do sistema cuida do resto.

🛠️ O que ele faz?
Registro Instantâneo: Digite "Gastei 50 no restaurante" ou "Caiu meu bônus de 200" e o sistema processa os dados em milissegundos.

Classificação Inteligente: Através da integração com o Gemini AI, o app identifica automaticamente se o gasto foi com Transporte, Lazer, Saúde ou Essenciais.

Dashboard em Tempo Real: Uma visão visual limpa (gráficos e indicadores) alimentada por um banco de dados Firebase, mostrando exatamente para onde seu dinheiro está indo.

Agente Financeiro Proativo: Mais que um banco de dados, o app atua como um mentor, enviando alertas quando você está prestes a estourar o orçamento de uma categoria.

💻 Diferenciais Técnicos
Arquitetura Serverless: Escalável e seguro usando Firebase Auth e Firestore.

NLP de Última Geração: Processamento de linguagem natural via Gemini 1.5 Flash.

Mobile-First: Design pensado para ser ágil, minimalista e acessível em qualquer lugar.

"VibeFinance: Porque controlar seu dinheiro deve ser tão fácil quanto gastar ele."

**Prints**

<img width="1347" height="628" alt="image" src="https://github.com/user-attachments/assets/210559a6-6dd3-4b13-bb49-2cd71dc56f93" />
<img width="856" height="516" alt="image" src="https://github.com/user-attachments/assets/27422270-0170-41b6-bfd4-bebe1a8609ac" />
<img width="845" height="445" alt="image" src="https://github.com/user-attachments/assets/927b11c4-23ae-4192-927d-fcbcda84b724" />
<img width="849" height="510" alt="image" src="https://github.com/user-attachments/assets/2b6bdc9b-0ce0-42a9-bc3f-465eb533258a" />

## 💬 Conclusão

Vibe Coding é sobre clareza, curiosidade e criatividade, não sobre perfeição técnica. O verdadeiro objetivo aqui é aprender a pensar junto com a IA, transformando ideias em conceitos reais e enxergando a tecnologia como uma extensão do seu raciocínio criativo. Cada interação é um experimento, quanto mais clara for sua intenção, mais surpreendente será o resultado.
