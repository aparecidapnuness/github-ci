# 📦 Testes de API - ViaCEP com Postman

Este repositório contém testes automatizados da API pública do [ViaCEP](https://viacep.com.br), realizados com o **Postman**. A proposta é simular consultas de CEPs de forma dinâmica, prática comum em testes de QA para validação de serviços REST.

---

## 🧪 O que foi testado?

- Consulta de diversos CEPs válidos.
- Verificação do retorno correto dos dados (logradouro, bairro, cidade, etc.).
- Validação de status code da resposta.

---

## ⚙️ Tecnologias utilizadas

- [Postman](https://www.postman.com/)
- Variáveis de ambiente dinâmicas em JavaScript (`pm.variables.set`)
- GitHub Actions para rodar os testes na pipeline CI

---

## 🚀 Como executar os testes

1. Clone o repositório ou acesse via GitHub.
2. Importe o arquivo `viacep-ci.json` no Postman (Collection).
3. Importe o arquivo `viacep-env.json` como ambiente.
4. Execute os testes com o **Collection Runner**.

> A variável `zipCode` é gerada aleatoriamente com uma função JavaScript e inserida nas requisições para simular testes variados.

---

## 🤖 CI - Integração Contínua

Os testes são executados automaticamente por meio do **GitHub Actions** sempre que há push no repositório.

---

## 👩‍💻 Sobre o projeto

Este projeto foi criado com o objetivo de praticar testes de API como QA Júnior, utilizando boas práticas de automação com Postman e integração com pipeline CI.
