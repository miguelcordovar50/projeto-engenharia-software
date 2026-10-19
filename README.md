# 🎮 GameVault — Hub de Gestão de Jogos e Clipes

## 1. Sobre o Projeto

O **GameVault** é uma plataforma digital desenvolvida para centralizar a biblioteca de jogos, o gerenciamento de clipes de gameplay e a troca de itens ou contas entre jogadores. A aplicação surge para resolver o problema de fragmentação que os gamers enfrentam: em vez de espalhar gravações, capturas de tela e listas de desejos em vários locais, o GameVault unifica tudo em um painel interativo, permitindo também que criadores de conteúdo organizem seus arquivos de vídeo e programem postagens para redes sociais.

---

## 2. Tecnologias, Ferramentas e Infraestrutura

Para sustentar a arquitetura do sistema, foram definidas as seguintes tecnologias:

* **Linguagens:** Python (Back-end / Automação) e JavaScript (Front-end).
* **Banco de Dados:** PostgreSQL (para armazenamento relacional de usuários, bibliotecas de jogos e metadados de vídeos).
* **Cloud & Hospedagem:** AWS (Amazon Web Services) para armazenamento de mídia (AWS S3 para os clipes e AWS EC2 para a API).
* **Controle de Versão:** Git e GitHub.
* **Ferramentas de Design / Interface:** Figma (para prototipagem das telas do sistema).

---

## 3. Metodologias Utilizadas

### 3.1 Modelo de Ciclo de Vida: Processo Iterativo e Incremental (ou Espiral)
Para o desenvolvimento do GameVault, escolhemos a **Metodologia Espiral / Iterativa**. 
* **Por quê?** Como o software envolve integração de player de vídeo, banco de dados relacional e painéis interativos, o modelo em cascata engessaria o projeto se houvesse mudança nos requisitos de mídia. A abordagem iterativa permite entregar o sistema em "fases" (v.1 com cadastro de jogos, v.2 com upload de clipes, v.3 com painel de métricas), mitigando riscos e permitindo testes contínuos a cada ciclo.

### 3.2 Uso do Git e GitHub
O versionamento de código e controle do projeto seguirão boas práticas colaborativas:
* **Branches (Ramos):** Uso da branch `main` apenas para versões estáveis em produção, branch `develop` para integração das funcionalidades, e branches de features (`feature/login`, `feature/upload-clipes`) para o desenvolvimento isolado de cada módulo.
* **Commits Semânticos:** Padronização das mensagens de commit (ex: `feat: adiciona tela de login`, `fix: corrige erro no banco de dados`, `docs: atualiza o readme`).
* **Pull Requests (PRs):** Code review obrigatório antes de mesclar novas funcionalidades na branch principal.

---

## 4. Projeto de Interface (Protótipos de Tela)

Abaixo estão descritas as principais telas projetadas no Figma para a experiência do usuário:

1. **Tela de Login / Cadastro:** Interface limpa com campos de e-mail, senha e botões de acesso rápido via redes sociais.
2. **Dashboard Principal (Home):** Painel central exibindo a biblioteca de jogos recentes do usuário, atalhos rápidos para os últimos clipes gravados e estatísticas de uso.
3. **Módulo de Gerenciamento de Clipes:** Tela focada na listagem de vídeos editados, com opções de pré-visualização, tags de jogos e status de renderização.
4. **Perfil do Usuário:** Configurações de conta, preferências de tema (modo escuro padrão) e links para redes sociais conectadas.

> *Dica: Você pode substituir esta seção ou adicionar imagens reais dos prints gerados no Figma salvos na pasta `/assets` do seu repositório.*

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/b5c7c5a1-c9d4-431e-8810-365c2a729a1e" />
