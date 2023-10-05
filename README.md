<div align="center"><img src="https://media.licdn.com/dms/image/C4D16AQElB0y1d5svPg/profile-displaybackgroundimage-shrink_200_800/0/1658867832742?e=2147483647&v=beta&t=i56I1rSG-TTCSP6hZbam6Wo9gwZINgRKqeXGKuCwP0w" tittle="compass.uol"></div>

# Automação de testes de API - Estágio QA Compass.UOL

Este é um projeto de automação da API ServeRest desenvolvido durante a Sprint 7 do programa de bolsas da empresa Compass.UOL. 

A proposta foi elaborar um plano de testes da API, utilizá-lo como base para criar testes utilizando o Postman, automatizar os testes criados, gerar relatório de execução e relatar possíveis bugs e melhorias.

## Mapa da API ServeRest

Você pode encontrar o arquivo do mapa [clicando aqui](/mapa-mental)

![ParaBank Map](/mapa-mental/API_ServeRest.png)

## Executar os testes no Postman

1. Certifique-se de ter o Postman instalado em seu sistema. Se não tiver, você pode baixá-lo e instalá-lo a partir do site oficial: [Postman](https://www.postman.com/).

2. Crie uma pasta onde você colocará os arquivos e abra um terminal do Git Bash a partir dela. Para isso você também precisa ter o [Git](https://git-scm.com/) instalado em seu computador.

3. Digite estes comandos no terminal para clonar os arquivos:
   ```
   git clone https://github.com/LuisDiasCompass/Sprint7_LuisDias_Compass.git

   ```

   Você também pode baixar o [arquivo zip](https://github.com/LuisDiasCompass/Sprint7_LuisDias_Compass/archive/refs/heads/main.zip) e descompactar na sua pasta.

4. Abra o Postman e importe os seguintes arquivos do repositório que você baixou que estão dentro da pasta 'postman':

   * ServeRest_postman_collection.json
   * Local_postman_environment.json
   * Web_postman_environment.json

5. Selecione um ambiente de execução no menu superior.
    
    Para executar no ambiente local você precisa rodar o servidor do ServeRest no seu computador, para isso siga os passos abaixo:
    * Instale o [Node.js](https://nodejs.org/en)
    * Abra o terminal do seu computador e rode o comando
    ```
        npx serverest@latest
    ```

6. Clique com o botão direito do mouse sobre a coleção 'ServeRest' e depois em 'Run collection'.

7. Na nova janela que será aberta selecione os cenários de teste que deseja executar e clique em 'Run ServeRest'.

## Executar testes no terminal

1. Para executar os testes através do terminal além do [Node.js](https://nodejs.org/en) você também precisara instalar o Newman. Para isso rode os seguintes comandos no seu terminal:
    ```
        npm install -g newman

    ```
    ```
        npm install -g newman-reporter-htmlextra

    ```

2. Após isso, navegue até a pasta do repositório e rode os testes com o comando:
    ```
        newman run ServeRest_postman_collection.json -e Local_postman_environment.json -r htmlextra --reporter-htmlextra-title "ServeRest API Test Report"

    ```

3. O relatório de execução estará na pasta 'postman/newman'.

## Referências
   
### Automação de Testes de API com Postman - Udemy
   * https://compassuol.udemy.com/course/automacao-de-testes-de-api-com-postman-projeto-de-testes/


## Conteúdo do Repositório

Este repositório contém códigos, exercícios e informações relacionados ao meu estágio no Studio Quality & Test Automation da Compass.UOL. Fique à vontade para utilizar e me enviar mensagem para dúvidas, feedbacks ou sugestões.

## Contato
### Luís Eduardo Dias, [Enviar e-mail](mailto:luis.dias.pb@compasso.com.br).
