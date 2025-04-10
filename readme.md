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

- **Endpoint:** `/completa-plus`
- **Método:** POST
- **Descrição:** Consulta Completa Plus.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes",
    "tipoPessoa": "J ou F"
  }
  ```

- **Endpoint:** `/serasaCredNet/pf`
- **Método:** POST
- **Descrição:** Consulta Serasa cred net para pessoa fisica.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/serasaCredNetBasica/pf`
- **Método:** POST
- **Descrição:** Consulta Serasa cred net basica para pessoa fisica.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/serasaCredNet/pj`
- **Método:** POST
- **Descrição:** Consulta Serasa cred net para pessoa juridica.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```

- **Endpoint:** `/serasaCredNetBasica/pj`
- **Método:** POST
- **Descrição:** Consulta Serasa cred net basica para pessoa juridica.
- **Body:**

  ```json
  {
    "doc": "cpf_sem_pontuacoes"
  }
  ```
