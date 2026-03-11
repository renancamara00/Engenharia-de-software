# 🖥️ Projeto plataforma de descontos de jogos

### Resumo

Plataforma agregadora de ofertas de jogos. Este repositório contém o desenvolvimento de uma solução para monitoramento de preços, permitindo registrar promoções, enviar alertas de descontos em tempo real e redirecionar o usuário diretamente para a loja de origem.

#

## 🛠️ Infraestrutura Técnica

### **Backend**
*   **Linguagem/Framework:** Node.js com NestJS (ou Python com FastAPI) para uma API escalável e de alto desempenho.
*   **Arquitetura:** RESTful API com suporte a Webhooks para integração com APIs de lojas (Steam, Epic, Nuuvem).
*   **Agendamento (Cron Jobs):** BullMQ ou Celery para verificação periódica de novos descontos.
*   **Web Scraping:** Puppeteer ou BeautifulSoup para extrair preços de lojas que não possuem API pública.

### **Frontend (Web)**
*   **Framework:** Next.js (recomendado para melhor indexação de SEO dos jogos e performance).
*   **Estilização:** Tailwind CSS para uma interface responsiva, moderna e otimizada.
*   **Gerenciamento de Estado:** TanStack Query (React Query) para sincronização de dados da API e gerenciamento de cache.

### **Mobile**
*   **Tecnologia:** React Native ou Flutter para desenvolvimento multiplataforma (iOS e Android).
*   **Notificações:** Firebase Cloud Messaging (FCM) para envio de alertas de promoções em tempo real.
*   **Deep Linking:** Configuração de links inteligentes para abrir o aplicativo diretamente na página do jogo desejado.

### **Banco de Dados**
*   **Relacional (Principal):** PostgreSQL para persistência de usuários, listas de desejos e histórico de preços.
*   **Não-Relacional (Cache):** Redis para armazenamento temporário de buscas e redução de carga no banco principal.
*   **Busca:** Meilisearch ou Elasticsearch para filtros ultrarrápidos por título, gênero ou plataforma.

#
