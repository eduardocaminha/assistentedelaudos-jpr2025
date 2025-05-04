# JPR 2025 HandsOn IA: Assistente de Geração de Laudos Radiológicos com Gemini

Este projeto foi desenvolvido como parte do **HandsOn IA da Jornada Paulista de Radiologia (JPR) 2025**, visando capacitar radiologistas na criação de assistentes inteligentes para geração automática e estruturada de laudos radiológicos e para geração de hipóteses diagnósticas, utilizando a plataforma Gemini do Google.

---

## Objetivos

- Ensinar os participantes a criar um assistente personalizado para gerar laudos precisos e consistentes.
- Ensinar os participantes a criar um assistente personalizado para elaboração de hipóteses diagnósticas em neurorradiologia.
- Demonstrar passo a passo, em tempo real, como configurar os assistentes no Gemini.
- Garantir que todos os participantes consigam criar e testar seus assistentes durante o HandsOn.

---

## Autores

- **Augusto Sarquis Serpa** - [LinkedIn](https://www.linkedin.com/in/augusto-sarquis-serpa-6aa8a3223/)
- **Eduardo Caminha Nunes** - [LinkedIn](https://www.linkedin.com/in/eduardocaminha/)
- **Eduardo Farina** - [LinkedIn](https://www.linkedin.com/in/eduardomjmfarina/)
- **Felipe Kitamura** - [LinkedIn](https://www.linkedin.com/in/felipekitamura/)
- **Julio Cesar Nather** - [LinkedIn](https://www.linkedin.com/in/julio-nather-049618181/)

---

## Pré-requisitos

Antes do início do HandsOn, certifique-se de possuir:

- Uma conta Google ativa.
- Acesso ao [Gemini](https://gemini.google.com/app).
- Todos os arquivos necessários estão disponibilizados no diretório "main" deste GitHub.

---

## Passo a Passo Detalhado

- Abra o navegador e vá para [Gemini](https://gemini.google.com/app).
- Realize o login com sua conta Google.
  
## Parte 1 - assistente de laudos

### 1.1. Testando o Gemini 2.0 "cru"

- Escreva no campo do _chat_, onde está escrito **"Peça ao Gemini"**, algum achado hipotético visualizado em uma tomografia de tórax que você está laudando.
- Peça para o Gemini gerar o laudo deste exame incluindo o achado que você relatou.
- Salve este _prompt_ que você criou em um bloco de notas no seu computador, pois ele será usado novamente mais tarde.
- Caso não possua conhecimentos médicos, iremos te auxiliar nessa parte.
- Aperte _Enter_ e analise a resposta do Gemini.
  
### 1.2. Criando o Assistente

- Clique em **"Gerenciador de Gem"**.
- Clique em **"Novo Gem"**

### 1.3. Configurando o Assistente

- Nomeie o assistente claramente como "Assistente de Laudos JPR2025".
- Localize o campo "Instruções".
- Abra o arquivo `instrucoes_assistente_laudos.txt` e analise o conteúdo.
- Caso concorde, copie o conteúdo e cole no campo de instruções no Gemini.
- Abra o arquivo `laudario.txt`, analise o conteúdo e faça o download do mesmo.
- Carregue o arquivo `laudario.txt` na seção "Conhecimento".

### 1.4. Salvando e Testando

- Clique em **"Salvar"** e depois em **"Iniciar conversa"**.
- Abra o bloco de notas e copie o seu _prompt_ anterior no campo do _chat_, onde está escrito **"Peça ao Gemini"**, e aperte _Enter_.
- Analise a nova resposta do Gemini.
- Após fornecer os dados solicitados, o assistente irá gerar automaticamente o laudo estruturado.
- Tente mudar o modelo no canto superior esquerdo para ver os resultados.
  
## Parte 2 - assistente de diagnósticos em neurorradiologia

### 2.1. Testando o Gemini 2.0 "cru"

- Abra o arquivo `prompt_neurorradio.txt` e analise o conteúdo. Trata-se de um caso clínico de um paciente com provável síndrome SMART com apresentação 5 anos após radioterapia para um tumor encefálico.


![image](https://github.com/user-attachments/assets/0adc2888-96e3-436c-b704-5ea0b0e7e47e) ![image](https://github.com/user-attachments/assets/bcca5861-023c-45ca-86c3-5cc0ae5b3f0a)

Imagem axial FLAIR evidenciando espessamento e alteração de sinal cortical temporo-occipital à direita e T1 pós-contraste evidencia realce giriforme nessa localização e tênue realce leptomeníngeo.

![image](https://github.com/user-attachments/assets/f4c082a7-c79c-4a5d-a712-8f119b7b55db) 

Imagens de controle após 2 semanas evidenciam redução do realce.


  
- Caso concorde com o prompt, copie o conteúdo e cole no campo do _chat_, onde está escrito **"Peça ao Gemini"**, e aperte _Enter_.
- Analise a resposta do Gemini.
  
### 2.2. Criando o Assistente

- Clique em **"Gerenciador de Gem"**.
- Clique em **"Novo Gem"**

### 2.3. Configurando o Assistente

- Nomeie o assistente claramente como "Neurorradiologista virtual JPR2025".
- Localize o campo "Instruções".
- Abra o arquivo `instrucoes_neurorradio.txt` e analise o conteúdo.
- Caso concorde, copie o conteúdo e cole no campo de instruções no Gemini.
- Baixe e carregue o arquivo `artigo.pdf` na seção "Conhecimento".

### 2.4. Salvando e Testando

- Clique em **"Salvar"** e depois em **"Iniciar conversa"**.
- Abra novamente o arquivo `prompt_neurorradio.txt` e copie o conteúdo e cole no campo do _chat_, onde está escrito **"Peça ao Gemini"**, e aperte _Enter_.
- Analise a nova resposta do Gemini.
- Tente mudar o modelo no canto superior esquerdo para ver os resultados.

## (BÔNUS) 3. Integrando os dois agentes em um só

### 3.1. Criando o Assistente

- Clique em **"Gerenciador de Gem"**.
- Clique em **"Novo Gem"**

### 3.2. Configurando o Assistente

- Nomeie o assistente claramente como "Assistente de laudos e neurorradiologista virtual JPR2025".
- Localize o campo "Instruções".
- Abra o arquivo `instrucoes_bonus.txt` e analise o conteúdo.
- Caso concorde, copie o conteúdo e cole no campo de instruções no Gemini.
- Carregue os arquivos `artigo.pdf` e `laudario.txt` na seção "Conhecimento".

### 3.3. Salvando e Testando

- Clique em **"Salvar"** e depois em **"Iniciar conversa"**.
- Abra o arquivo `prompt_bonus.txt` e copie o conteúdo e cole no campo do _chat_, onde está escrito **"Peça ao Gemini"**, e aperte _Enter_.
- Analise a resposta do Gemini.
- Tente mudar o modelo no canto superior esquerdo para ver os resultados.

## Dicas Importantes

- Sempre responda exatamente ao solicitado pelo assistente para garantir precisão.
- Utilize termos médicos corretos para otimizar os resultados.

---

## Suporte e Dúvidas

Durante o HandsOn, os autores estarão disponíveis para solucionar dúvidas e fornecer suporte individual.

---
