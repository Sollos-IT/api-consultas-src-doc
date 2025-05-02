# API Consultas

Esta documentação descreve as rotas disponíveis na API de consultas. Todas as requisições POST devem incluir um `x-access-token` no header, que é obtido através da rota `/login` informando o usuário e senha.

## Autenticação

### Login

- **Endpoint:** `/login`
- **Método:** POST
- **Descrição:** Autentica o usuário e retorna um token de acesso.
- **Body:**
  ```json
  {
    "user": "seu_usuario",
    "password": "sua_senha"
  }
  ```

## Consultas

### SRC

- **Endpoint:** `/src/pf-pj`
- **Método:** POST
- **Descrição:** Consulta SRC.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/src-score/pf-pj`
- **Método:** POST
- **Descrição:** Consulta SRC + SCORE.
- **Body:**
  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

### Consultas Diversas

- **Endpoint:** `/boa-vista-scpc-score`
- **Método:** POST
- **Descrição:** boa vista scpc score.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes",
    "tipoPessoa": "J ou F"
  }
  ```

- **Endpoint:** `/ccf-protesto-nacional`
- **Método:** POST
- **Descrição:** Consulta CCF protesto nacional.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/consulta-integrador`
- **Método:** POST
- **Descrição:** Consulta integrador.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/protesto-nacional`
- **Método:** POST
- **Descrição:** Consulta protesto nacional.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/relatorio-basico-score-cpf`
- **Método:** POST
- **Descrição:** Consulta de relatorio basico score para cpf.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/serasa-cnpj`
- **Método:** POST
- **Descrição:** Consulta de serasa para CNPJ.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/serasa-score-cpf`
- **Método:** POST
- **Descrição:** Consulta de serasa + score para CPF.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```
