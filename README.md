# 🖥️ Projeto plataforma de descontos de jogos

### Resumo

Plataforma agregadora de ofertas de jogos. Este repositório contém o desenvolvimento de uma solução para monitoramento de preços, permitindo registrar promoções, enviar alertas de descontos em tempo real e redirecionar o usuário diretamente para a loja de origem.

#

## 🛠️ Infraestrutura Técnica

### **Backend**
*   **Linguagem/Framework:** Node.js com NestJS (ou Python com FastAPI). 
*   **Arquitetura:** RESTful API. 
*   **Agendamento (Cron Jobs):** BullMQ ou Celery. 
*   **Web Scraping:** Puppeteer ou BeautifulSoup. 

### **Frontend (Web)**
*   **Framework:** Next.js. 
*   **Estilização:** Tailwind CSS. 
*   **Gerenciamento de Estado:** TanStack Query (React Query).

### **Mobile**
*   **Tecnologia:** React Native ou Flutter. 
*   **Notificações:** Firebase Cloud Messaging (FCM). 
*   **Deep Linking:** Configuração de links inteligentes para abrir o aplicativo diretamente na página do jogo desejado.

### **Banco de Dados**
*   **Relacional (Principal):** PostgreSQL.
*   **Não-Relacional (Cache):** Redis.
*   **Busca:** Meilisearch ou Elasticsearch.

#
