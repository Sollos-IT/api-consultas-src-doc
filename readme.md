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

### Consultas Restritivas
- **Endpoint:** `/restritivo-cadastral/pf`
- **Método:** POST
- **Descrição:** Consulta restritiva cadastral para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/restritivo-cadastral/pj`
- **Método:** POST
- **Descrição:** Consulta restritiva cadastral para pessoa jurídica.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

### Consultas de Situação Cadastral
- **Endpoint:** `/situacao-cadastral/pf`
- **Método:** POST
- **Descrição:** Consulta situação cadastral federal para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Óbito
- **Endpoint:** `/obito-flag/pf`
- **Método:** POST
- **Descrição:** Consulta flag de óbito para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/obito/pf`
- **Método:** POST
- **Descrição:** Consulta de óbito para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Participações Societárias
- **Endpoint:** `/participacoes-societarias/pf`
- **Método:** POST
- **Descrição:** Consulta participações societárias para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de PEP
- **Endpoint:** `/pep/pf`
- **Método:** POST
- **Descrição:** Consulta PEP para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de OFAC
- **Endpoint:** `/ofac/pf`
- **Método:** POST
- **Descrição:** Consulta OFAC para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Sanções e Restrições
- **Endpoint:** `/sancaoes-restricoes/pf`
- **Método:** POST
- **Descrição:** Consulta sanções e restrições para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas KYC Ampliado
- **Endpoint:** `/kyc-ampliado/pf`
- **Método:** POST
- **Descrição:** Consulta KYC ampliado para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Biometria Facial
- **Endpoint:** `/biometria-facial/pf`
- **Método:** POST
- **Descrição:** Consulta biometria facial para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes",
        "selfie": "selfie_base64",
    }
    ```

### Consultas de Processos
- **Endpoint:** `/processos-basico/pf`
- **Método:** POST
- **Descrição:** Consulta processos básicos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/processos-amplificados/pf`
- **Método:** POST
- **Descrição:** Consulta processos amplificados para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Programas de Benefício e Assistência Social
- **Endpoint:** `/programas-de-beneficio-e-assistencia-social/pf`
- **Método:** POST
- **Descrição:** Consulta programas de benefício e assistência social para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Notícias e Mídia
- **Endpoint:** `/noticias-midia/pf`
- **Método:** POST
- **Descrição:** Consulta notícias e mídia para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Pessoas do Esporte
- **Endpoint:** `/pessoas-do-esporte/pf`
- **Método:** POST
- **Descrição:** Consulta pessoas do esporte para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Veículos
- **Endpoint:** `/busca-veiculos/pf`
- **Método:** POST
- **Descrição:** Consulta veículos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Familiares e Conhecidos
- **Endpoint:** `/familiares/conhecidos/pf`
- **Método:** POST
- **Descrição:** Consulta familiares e conhecidos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Familiares PEP
- **Endpoint:** `/familiares/pep/pf`
- **Método:** POST
- **Descrição:** Consulta familiares PEP para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Familiares OFAC
- **Endpoint:** `/familiares/ofac/pf`
- **Método:** POST
- **Descrição:** Consulta familiares OFAC para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Familiares com Sanções e Restrições
- **Endpoint:** `/familiares/sancaoes-restricoes/pf`
- **Método:** POST
- **Descrição:** Consulta familiares com sanções e restrições para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Familiares com Processos
- **Endpoint:** `/familiares/processos/pf`
- **Método:** POST
- **Descrição:** Consulta familiares com processos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas por Nome
- **Endpoint:** `/nome/noticias-midias/pf`
- **Método:** POST
- **Descrição:** Consulta notícias e mídia por nome para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas AOB
- **Endpoint:** `/aob/cadastral-receita-federal/pf`
- **Método:** POST
- **Descrição:** Consulta cadastral na Receita Federal para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/aob/cadastral/pf`
- **Método:** POST
- **Descrição:** Consulta cadastral na AOB para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

### Consultas de Documentos
- **Endpoint:** `/documentos/ocr/pf`
- **Método:** POST
- **Descrição:** Consulta OCR de documentos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes",
        "image": "image_base64",
    }
    ```

- **Endpoint:** `/documentos/autenticacao/pf`
- **Método:** POST
- **Descrição:** Consulta de autenticação de documentos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes",
        "image": "image_base64",
    }
    ```

- **Endpoint:** `/documentos/autenticacao-pro/pf`
- **Método:** POST
- **Descrição:** Consulta de autenticação pro de documentos para pessoa física.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes",
        "image": "image_base64",
    }
    ```

### Consultas de CNPJ
- **Endpoint:** `/buscar-veiculos/cnpj`
- **Método:** POST
- **Descrição:** Consulta veículos para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes",
  
    }
    ```

- **Endpoint:** `/faturamento-presumido/cnpj`
- **Método:** POST
- **Descrição:** Consulta faturamento presumido para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/kyc-ampliado/cnpj`
- **Método:** POST
- **Descrição:** Consulta KYC ampliado para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/ofac/cnpj`
- **Método:** POST
- **Descrição:** Consulta OFAC para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/participacoes-societarias/cnpj`
- **Método:** POST
- **Descrição:** Consulta participações societárias para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/processos-basicos/cnpj`
- **Método:** POST
- **Descrição:** Consulta processos básicos para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/processos-ampliado/cnpj`
- **Método:** POST
- **Descrição:** Consulta processos ampliados para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/sacoes-restricoes/cnpj`
- **Método:** POST
- **Descrição:** Consulta sanções e restrições para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/sintegra/cnpj`
- **Método:** POST
- **Descrição:** Consulta Sintegra para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/situacao-cadastral-federal/cnpj`
- **Método:** POST
- **Descrição:** Consulta situação cadastral federal para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/socios/pep/cnpj`
- **Método:** POST
- **Descrição:** Consulta sócios PEP para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/socios/processos/cnpj`
- **Método:** POST
- **Descrição:** Consulta sócios com processos para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

### Consultas Diversas
- **Endpoint:** `/boa-vista-scpc-score`
- **Método:** POST
- **Descrição:** Consulta Boa Vista SCPC Score.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/ccf-protesto-nacional`
- **Método:** POST
- **Descrição:** Consulta CCF Protesto Nacional.
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
- **Descrição:** Consulta relatório básico score CPF.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/serasa-cnpj`
- **Método:** POST
- **Descrição:** Consulta Serasa para CNPJ.
- **Body:**
    ```json
    {
        "doc": "cnpj_sem_pontuacoes"
    }
    ```

- **Endpoint:** `/serasa-score-cpf`
- **Método:** POST
- **Descrição:** Consulta Serasa Score para CPF.
- **Body:**
    ```json
    {
        "doc": "cpf_sem_pontuacoes"
    }
    ```
