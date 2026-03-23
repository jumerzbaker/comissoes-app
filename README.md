Comissões App
Sistema web de controle de comissões de vendas, desenvolvido para uso real em ambiente empresarial.

🔗 Acesse o app ao vivo

📌 Sobre o projeto
O Comissões App é uma aplicação web completa para gestão de comissões de equipes de vendas. Foi desenvolvido para uso real por uma empresa, substituindo o controle manual em planilhas por um sistema moderno, acessível em qualquer dispositivo e com dados sincronizados em tempo real.

O projeto nasceu de uma necessidade real: uma equipe com mais de 5 vendedores precisava de uma forma simples e centralizada de acompanhar vendas, calcular comissões automaticamente e visualizar relatórios de desempenho — tudo pelo celular ou computador.

✨ Funcionalidades
Dashboard com KPIs em tempo real — total vendido, comissões pagas e a receber
Controle de vendas — registro de vendas com cálculo automático de comissão
Regras flexíveis de comissão — % padrão por tipo e % especial por produto específico
Cadastro de vendedores com totais calculados automaticamente
Relatórios completos — visão geral, individual por vendedor e ranking comparativo
Sincronização em tempo real — alterações aparecem instantaneamente para todos os usuários
Interface responsiva — experiência nativa em celular e desktop
Marcar comissões como pagas — controle do status de cada pagamento
🛠️ Tecnologias utilizadas
Tecnologia	Uso
HTML5	Estrutura da aplicação
CSS3	Estilização e responsividade (mobile-first)
JavaScript (ES6+)	Lógica da aplicação, manipulação de DOM
Firebase Firestore	Banco de dados NoSQL em tempo real
Firebase SDK v11	Integração com serviços do Google
GitHub Pages	Hospedagem gratuita em produção
📱 Layout
O app foi projetado com abordagem mobile-first, adaptando-se automaticamente a qualquer tamanho de tela:

Desktop — sidebar de navegação, tabelas completas, gráfico de barras
Mobile — navegação inferior, cards de conteúdo, botão flutuante de ação (FAB)
🏗️ Arquitetura
comissoes-app/
└── index.html          # Aplicação completa (SPA em arquivo único)
                        ├── Estilos CSS (mobile-first, variáveis CSS)
                        ├── HTML (estrutura e modais)
                        └── JavaScript
                            ├── Firebase SDK (módulos ESM)
                            ├── Listeners em tempo real (onSnapshot)
                            ├── Renderização dinâmica de páginas
                            └── CRUD completo via Firestore
A aplicação é uma SPA (Single Page Application) construída em vanilla JS, sem frameworks, demonstrando domínio dos fundamentos da web.

🔥 Integração com Firebase
O app utiliza o Firebase Firestore com listeners em tempo real (onSnapshot), o que significa que qualquer alteração feita por um usuário é refletida instantaneamente na tela de todos os outros usuários conectados — sem necessidade de recarregar a página.

Coleções no Firestore:

vendedores — cadastro da equipe de vendas
comissoes — tipos e regras de comissionamento
vendas — registro de todas as vendas realizadas
🚀 Como executar localmente
Por ser um arquivo HTML único, não há necessidade de instalação ou build:

# Clone o repositório
git clone https://github.com/jumerzbaker/comissoes-app.git

# Abra o arquivo no navegador
open index.html
⚠️ Para a integração com Firebase funcionar, é necessário ter um projeto Firebase com Firestore habilitado e substituir as credenciais no arquivo index.html.

📊 Decisões técnicas
Por que vanilla JS e não React/Vue? A escolha foi intencional: demonstrar domínio dos fundamentos do JavaScript puro antes de abstrações de frameworks. O resultado é uma aplicação leve, sem dependências de build e com carregamento instantâneo.

Por que Firebase Firestore? Por ser uma solução BaaS (Backend as a Service) que elimina a necessidade de um servidor próprio, permitindo focar na experiência do usuário. O Firestore oferece sincronização em tempo real nativa, ideal para múltiplos usuários simultâneos.

Por que arquivo único? Facilita a distribuição e hospedagem — qualquer pessoa pode abrir o arquivo localmente ou hospedar em qualquer serviço estático, sem configuração de servidor.

🔮 Próximos passos
 Autenticação de usuários (Firebase Auth)
 Controle de acesso por perfil (admin / vendedor)
 Exportação de relatórios em PDF
 Notificações de novas vendas
 Modo offline com sincronização posterior
👩‍💻 Autora
Júlia Merzbaker Migrando para a área de tecnologia com foco em desenvolvimento web.

LinkedIn GitHub

📄 Licença
Este projeto foi desenvolvido para uso empresarial privado. O código é disponibilizado publicamente para fins de portfólio.

Feito com 💚 e muito JavaScript
