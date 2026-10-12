📉 Burndown Dashboard

Um painel que mostra o progresso de um sprint e recalcula a data de entrega conforme o ritmo real do time.

Mostrar Imagem

💡 Por que isso existe

Prever com precisão quanto tempo um projeto de software vai levar continua sendo (quase) impossível. Software é descoberta, não manufatura: requisitos mudam, imprevistos técnicos surgem e a complexidade cresce de forma não linear.

Este projeto não tenta resolver o problema. Ele mostra o problema: a cada registro de progresso, a data prevista muda. A linha "ideal" quase nunca bate com a linha "real".

✨ Funcionalidades
🗓️ Cadastro do sprint (início, fim e total de pontos)
✅ Registro diário de pontos concluídos
📊 Gráfico com três linhas: ideal, real e projeção
🎯 Data de entrega prevista, com indicação de atraso ou adiantamento
💾 Dados salvos no navegador (localStorage), sem backend
🧮 Como a projeção funciona
ritmo real     = pontos concluídos ÷ dias decorridos
dias restantes = pontos restantes ÷ ritmo real
entrega        = hoje + dias restantes

Simples de propósito: o resultado muda todo dia, e é isso que ilustra a incerteza.

🛠️ Tecnologias
React
Vite
Tailwind CSS
Recharts
🚀 Como rodar
bash
# clonar o repositório
git clone https://github.com/SEU-USUARIO/burndown.git
cd burndown

# instalar as dependências
npm install

# iniciar em modo de desenvolvimento
npm run dev

Depois é só abrir o endereço que aparecer no terminal (normalmente http://localhost:5173).

🧪 Como testar
Crie um sprint de 10 dias com 40 pontos.
Registre alguns pontos concluídos em datas diferentes.
Observe a linha laranja (projeção) mudar a cada registro.
🗺️ Próximos passos
 Exportar o gráfico como imagem
 Suporte a vários sprints
 Modo escuro
 Simulação Monte Carlo para mostrar probabilidades em vez de uma data única
📄 Licença

Distribuído sob a licença MIT.
