# Nome do Projeto: cypress-actions (public)  
[https://github.com/viniciuscarneironascimento/cypress-actions](https://github.com/viniciuscarneironascimento/cypress-actions)

---

## 📝 Descrição  
Repositório do treinamento de automação de testes em Cypress com **integração contínua (CI/CD)** utilizando **Github Actions**. Treinamento ministrado pelo instrutor Fernando Papito.

---

## 🚀 Resultados Alcançados  
- Foco na criação de **workflows no GitHub Actions**, desde modelos simples até abordagens avançadas de integração contínua, com ênfase em pipelines de execução **paralela (shards)** e integração com o **Cypress Cloud**.  
- Criação de workflows manuais usando `workflow_dispatch`.  
- Uso do modo de gravação do Cypress Cloud (`record: true`) para envio dos resultados.

---

## ✅ Onde o `npx cypress run` é executado?  
Ele é executado dentro da GitHub Action usada aqui:
yaml
CopiarEditar
uses: cypress-io/github-action@v6.5.0
Essa Action oficial do Cypress já vem com lógica interna para rodar o Cypress da seguinte forma:
•	Se você não especificar outro comando, ela automaticamente executa:
bash
CopiarEditar
npx cypress run
•	Quando você define record: true, ela faz:
bash
CopiarEditar
npx cypress run --record --key <sua_record_key>
Ou seja, a Action abstrai esse comando, mas é isso que está sendo executado por baixo dos panos.


---


![poster](./.github/poster.png)

## Sobre

Repositório do treinamento: Workflow de testes contínuos em Cypress no Github Actions

## Stacks
- Cypress
- Javascript
- Cypress Dashboard
- Tesults

## Rodando

1. Clonar o repositório, instalar as dependências
```
yarn / npm install
```

2. Subir o Cypress UI
```
yarn cypress open / npx cypress open 
```

3. Executar testes em Headless
```
yarn cypress run / npx cypress run 
```

<hr>
Curso disponível em https://qaxperience.com

