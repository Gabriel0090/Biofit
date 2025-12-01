# BioFit - Programa de Acompanhamento de Saúde

Este projeto é um aplicativo de acompanhamento de saúde e fitness, desenvolvido como parte da disciplina de Laboratório de Engenharia de Software. Ele permite ao usuário gerenciar seu perfil pessoal e calcular diversas métricas corporais e nutricionais.

O projeto foi criado com **React** e **Vite**.

## Autores

* Arthur Zimmermann
* Gabriel Molinari
* Rafaella Gonçalves
* Sabrina Bloedow

## Funcionalidades Principais

Conforme a documentação do projeto e a implementação atual, as principais funcionalidades incluem:

1.  **Gerenciamento de Perfil:**
    * Cadastro de usuário com nome, email, sexo, idade, peso, altura e objetivo.
    * Edição dos dados pessoais.
    * Exibição de um resumo rápido na tela de perfil, incluindo IMC e peso atual.

2.  **Cálculos e Métricas Corporais:**
    * **IMC:** Cálculo do Índice de Massa Corporal.
    * **TMB:** Cálculo da Taxa Metabólica Basal (calorias diárias).
    * **Calorias Objetivas:** Cálculo de déficit ou superávit calórico baseado no objetivo do usuário.
    * **Creatina:** Cálculo da dose de manutenção recomendada com base no peso.

3.  **Cálculo de Macronutrientes:**
    * Calcula a distribuição ideal de proteínas, carboidratos e gorduras com base no gasto calórico diário e no objetivo do usuário.

4.  **Nutri IA (Assistente Virtual):**
    * Chatbot integrado que utiliza o modelo Gemini (gemini-2.5-flash) para responder a dúvidas de nutrição e fitness, usando o perfil do usuário como contexto.

5.  **Histórico de Evolução:**
    * Permite salvar os resultados de Cálculos e Macros para acompanhar a evolução do usuário ao longo do tempo.

## Estrutura do Projeto

O projeto utiliza uma estrutura padrão de aplicações React, separando componentes reutilizáveis e páginas.

## Tecnologias Utilizadas

* **Vite:** Build tool e servidor de desenvolvimento.
* **React:** Biblioteca principal para a UI.
* **React Router DOM:** Para gerenciamento de rotas (navegação entre páginas).
* **Gemini API:** Para integração com o assistente Nutri IA.
* **JSON Server:** Usado para simular um backend REST API simples (`db.json`) para persistência de dados de usuários e histórico.
* **React Toastify:** Para notificações e feedback ao usuário.
* **ESLint:** Ferramenta para linting e padronização de código.
* **Prop-types:** Para validação de tipos das props nos componentes React.

## Scripts Disponíveis

No diretório do projeto, você pode executar os seguintes comandos:

### `npm run server`

**Inicia o servidor de backend simulado (JSON Server) na porta 3000**. É necessário rodar este comando em um terminal separado para que o login, cadastro e persistência de dados funcionem.

### `npm run dev`

Executa o aplicativo em modo de desenvolvimento.
Abra [http://localhost:5173](http://localhost:5173) (ou a porta indicada no terminal) para visualizá-lo no navegador.

### `npm run build`

Compila o aplicativo para produção na pasta `dist/`.

### `npm run lint`

Executa o ESLint para analisar o código e encontrar problemas de formatação ou erros.

### `npm run preview`

Inicia um servidor local para pré-visualizar a versão de produção (após executar `npm run build`).