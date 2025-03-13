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

- **Endpoint:** `/restritivo-cadastral/pj`
- **Método:** POST
- **Descrição:** Consulta restritiva cadastral para pessoa jurídica.

### Consultas de Situação Cadastral
- **Endpoint:** `/situacao-cadastral/pf`
- **Método:** POST
- **Descrição:** Consulta situação cadastral federal para pessoa física.

### Consultas de Óbito
- **Endpoint:** `/obito-flag/pf`
- **Método:** POST
- **Descrição:** Consulta flag de óbito para pessoa física.

- **Endpoint:** `/obito/pf`
- **Método:** POST
- **Descrição:** Consulta de óbito para pessoa física.

### Consultas de Participações Societárias
- **Endpoint:** `/participacoes-societarias/pf`
- **Método:** POST
- **Descrição:** Consulta participações societárias para pessoa física.

### Consultas de PEP
- **Endpoint:** `/pep/pf`
- **Método:** POST
- **Descrição:** Consulta PEP para pessoa física.

### Consultas de OFAC
- **Endpoint:** `/ofac/pf`
- **Método:** POST
- **Descrição:** Consulta OFAC para pessoa física.

### Consultas de Sanções e Restrições
- **Endpoint:** `/sancaoes-restricoes/pf`
- **Método:** POST
- **Descrição:** Consulta sanções e restrições para pessoa física.

### Consultas KYC Ampliado
- **Endpoint:** `/kyc-ampliado/pf`
- **Método:** POST
- **Descrição:** Consulta KYC ampliado para pessoa física.

### Consultas de Biometria Facial
- **Endpoint:** `/biometria-facial/pf`
- **Método:** POST
- **Descrição:** Consulta biometria facial para pessoa física.

### Consultas de Processos
- **Endpoint:** `/processos-basico/pf`
- **Método:** POST
- **Descrição:** Consulta processos básicos para pessoa física.

- **Endpoint:** `/processos-amplificados/pf`
- **Método:** POST
- **Descrição:** Consulta processos amplificados para pessoa física.

### Consultas de Programas de Benefício e Assistência Social
- **Endpoint:** `/programas-de-beneficio-e-assistencia-social/pf`
- **Método:** POST
- **Descrição:** Consulta programas de benefício e assistência social para pessoa física.

### Consultas de Notícias e Mídia
- **Endpoint:** `/noticias-midia/pf`
- **Método:** POST
- **Descrição:** Consulta notícias e mídia para pessoa física.

### Consultas de Pessoas do Esporte
- **Endpoint:** `/pessoas-do-esporte/pf`
- **Método:** POST
- **Descrição:** Consulta pessoas do esporte para pessoa física.

### Consultas de Veículos
- **Endpoint:** `/busca-veiculos/pf`
- **Método:** POST
- **Descrição:** Consulta veículos para pessoa física.

### Consultas de Familiares e Conhecidos
- **Endpoint:** `/familiares/conhecidos/pf`
- **Método:** POST
- **Descrição:** Consulta familiares e conhecidos para pessoa física.

### Consultas de Familiares PEP
- **Endpoint:** `/familiares/pep/pf`
- **Método:** POST
- **Descrição:** Consulta familiares PEP para pessoa física.

### Consultas de Familiares OFAC
- **Endpoint:** `/familiares/ofac/pf`
- **Método:** POST
- **Descrição:** Consulta familiares OFAC para pessoa física.

### Consultas de Familiares com Sanções e Restrições
- **Endpoint:** `/familiares/sancaoes-restricoes/pf`
- **Método:** POST
- **Descrição:** Consulta familiares com sanções e restrições para pessoa física.

### Consultas de Familiares com Processos
- **Endpoint:** `/familiares/processos/pf`
- **Método:** POST
- **Descrição:** Consulta familiares com processos para pessoa física.

### Consultas por Nome
- **Endpoint:** `/nome/noticias-midias/pf`
- **Método:** POST
- **Descrição:** Consulta notícias e mídia por nome para pessoa física.

### Consultas AOB
- **Endpoint:** `/aob/cadastral-receita-federal/pf`
- **Método:** POST
- **Descrição:** Consulta cadastral na Receita Federal para pessoa física.

- **Endpoint:** `/aob/cadastral/pf`
- **Método:** POST
- **Descrição:** Consulta cadastral na AOB para pessoa física.

### Consultas de Documentos
- **Endpoint:** `/documentos/ocr/pf`
- **Método:** POST
- **Descrição:** Consulta OCR de documentos para pessoa física.

- **Endpoint:** `/documentos/autenticacao/pf`
- **Método:** POST
- **Descrição:** Consulta de autenticação de documentos para pessoa física.

- **Endpoint:** `/documentos/autenticacao-pro/pf`
- **Método:** POST
- **Descrição:** Consulta de autenticação pro de documentos para pessoa física.

### Consultas de CNPJ
- **Endpoint:** `/buscar-veiculos/cnpj`
- **Método:** POST
- **Descrição:** Consulta veículos para CNPJ.

- **Endpoint:** `/faturamento-presumido/cnpj`
- **Método:** POST
- **Descrição:** Consulta faturamento presumido para CNPJ.

- **Endpoint:** `/kyc-ampliado/cnpj`
- **Método:** POST
- **Descrição:** Consulta KYC ampliado para CNPJ.

- **Endpoint:** `/ofac/cnpj`
- **Método:** POST
- **Descrição:** Consulta OFAC para CNPJ.

- **Endpoint:** `/participacoes-societarias/cnpj`
- **Método:** POST
- **Descrição:** Consulta participações societárias para CNPJ.

- **Endpoint:** `/processos-basicos/cnpj`
- **Método:** POST
- **Descrição:** Consulta processos básicos para CNPJ.

- **Endpoint:** `/processos-ampliado/cnpj`
- **Método:** POST
- **Descrição:** Consulta processos ampliados para CNPJ.

- **Endpoint:** `/sacoes-restricoes/cnpj`
- **Método:** POST
- **Descrição:** Consulta sanções e restrições para CNPJ.

- **Endpoint:** `/sintegra/cnpj`
- **Método:** POST
- **Descrição:** Consulta Sintegra para CNPJ.

- **Endpoint:** `/situacao-cadastral-federal/cnpj`
- **Método:** POST
- **Descrição:** Consulta situação cadastral federal para CNPJ.

- **Endpoint:** `/socios/pep/cnpj`
- **Método:** POST
- **Descrição:** Consulta sócios PEP para CNPJ.

- **Endpoint:** `/socios/processos/cnpj`
- **Método:** POST
- **Descrição:** Consulta sócios com processos para CNPJ.

### Consultas Diversas
- **Endpoint:** `/boa-vista-scpc-score`
- **Método:** POST
- **Descrição:** Consulta Boa Vista SCPC Score.

- **Endpoint:** `/ccf-protesto-nacional`
- **Método:** POST
- **Descrição:** Consulta CCF Protesto Nacional.

- **Endpoint:** `/consulta-integrador`
- **Método:** POST
- **Descrição:** Consulta integrador.

- **Endpoint:** `/protesto-nacional`
- **Método:** POST
- **Descrição:** Consulta protesto nacional.

- **Endpoint:** `/relatorio-basico-score-cpf`
- **Método:** POST
- **Descrição:** Consulta relatório básico score CPF.

- **Endpoint:** `/serasa-cnpj`
- **Método:** POST
- **Descrição:** Consulta Serasa para CNPJ.

- **Endpoint:** `/serasa-score-cpf`
- **Método:** POST
- **Descrição:** Consulta Serasa Score para CPF.
