# Overview

Esse projeto simula o sistema de verificação pré-decolagem de uma nave espacial. Basicamente, o programa pede pra você digitar os dados atuais da nave (energia, temperatura interna e externa, pressão dos tanques, integridade estrutural e status dos módulos críticos), confere se tudo está dentro dos limites seguros e te diz se a nave está **pronta pra decolar** ou se a **decolagem precisa ser abortada** — e por quê. Se estiver tudo certo, ele ainda calcula quanto de energia sobra depois da decolagem e por quantas horas a nave consegue se manter operando.

## Tecnologias usadas

- Python 3.10+
- Jupyter Notebook

## Pré-requisitos

Pra rodar na sua máquina, você vai precisar ter instalado:

- Python 3.10 ou superior
- Git
- Jupyter Notebook (ou uma extensão que rode `.ipynb`, tipo a do VS Code)

## Como rodar

1. Clone o repositório:
   ```
   git clone https://github.com/Turatz/fiap-fase-1.git
   ```

2. Abra o arquivo `NotebookPython.ipynb`, que está dentro da pasta `fase 1`, no Jupyter Notebook, VS Code ou no editor que você preferir.

3. Rode todas as células do notebook em ordem.

4. O programa vai te pedir pra preencher alguns dados. Fique de olho nos limites abaixo, porque se algum valor sair da faixa, a decolagem é abortada:

   ![Alt text](https://i.imgur.com/QLvgnnj.png)

   - Energia: mínimo de 20%
   - Temperatura externa: entre 0 e 45ºC
   - Temperatura interna: entre 15 e 35ºC
   - Pressão dos tanques: entre 100 e 145 bar
   - Integridade estrutural: 0 (negativo) ou 1 (positivo)
   - Status dos módulos críticos: 0 (falha) ou 1 (ok)

   ![Alt text](https://i.imgur.com/jdGIJeA.png)

5. Se algum requisito falhar, o programa mostra exatamente qual foi o problema e pergunta se você quer tentar de novo:

   ![Alt text](https://i.imgur.com/USAnMgS.png)

6. Se tudo estiver dentro do esperado, ele libera a decolagem e já calcula a autonomia energética da nave (energia disponível, perdas, energia líquida e quantas horas de autonomia sobram):

   ![Alt text](https://i.imgur.com/czO2pTz.png)

## Licença

Esse programa não tem licença.
