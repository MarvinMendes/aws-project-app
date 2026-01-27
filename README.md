# ☁️ AWS Practice Lab

Bem-vindo ao meu repositório de estudos de **Amazon Web Services (AWS)**. O objetivo deste projeto é documentar a implementação prática, configurações e integrações entre os principais serviços da nuvem da Amazon.

---

## 🛠️ Serviços Explorados

Abaixo, detalho cada serviço utilizado neste laboratório e seu papel na arquitetura:

### 🗳️ Amazon S3 (Simple Storage Service)

Serviço de armazenamento de objetos que oferece escalabilidade, disponibilidade de dados, segurança e performance.

* **Uso no projeto:** Armazenamento de arquivos estáticos, logs de execução e backups de banco de dados.
* **Conceitos chave:** Buckets, Políticas de Acesso (IAM), e Versionamento.

### 💻 Amazon EC2 (Elastic Compute Cloud)

Capacidade de computação redimensionável na nuvem. São máquinas virtuais (instâncias) onde rodamos nossas aplicações.

* **Uso no projeto:** Hospedagem de um servidor web Linux para processamento de requisições pesadas.
* **Conceitos chave:** Security Groups, Key Pairs e Tipos de Instância.

### 🗄️ Amazon RDS (Relational Database Service)

Serviço gerenciado que facilita a configuração, operação e escalabilidade de bancos de dados relacionais.

* **Uso no projeto:** Persistência de dados estruturados utilizando o motor **PostgreSQL/MySQL**.
* **Conceitos chave:** Multi-AZ para alta disponibilidade e Subnet Groups.

### ⚡ AWS Lambda

Serviço de computação *serverless* que executa seu código em resposta a eventos sem a necessidade de gerenciar servidores.

* **Uso no projeto:** Funções auxiliares para redimensionamento de imagens e gatilhos de banco de dados.
* **Conceitos chave:** Triggers, Handlers e Runtime.

### 🌐 Amazon API Gateway

Serviço totalmente gerenciado que permite criar, publicar e manter APIs RESTful e WebSocket em qualquer escala.

* **Uso no projeto:** Porta de entrada para as funções Lambda, expondo endpoints HTTP para o front-end.
* **Conceitos chave:** Recursos (Resources), Métodos (GET/POST) e Autorizadores.

### 📥 Amazon SQS (Simple Queue Service)

Serviço de filas de mensagens gerenciado para desacoplar e dimensionar microsserviços e sistemas distribuídos.

* **Uso no projeto:** Garantir que nenhuma mensagem seja perdida durante picos de tráfego, armazenando tarefas para processamento assíncrono.
* **Conceitos chave:** Standard vs FIFO Queues e Dead Letter Queues (DLQ).

### 🔔 Amazon SNS (Simple Notification Service)

Serviço de mensagens Pub/Sub (Publicador/Assinante) para mensagens de alta throughput e entrega por push.

* **Uso no projeto:** Notificação imediata via E-mail ou SMS sempre que um erro crítico ocorre no sistema.
* **Conceitos chave:** Tópicos, Assinaturas (Subscriptions) e Fan-out.
