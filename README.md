# DESAFIO-QA-BEEDOO-2026

Repositório criado para a realização do **Desafio Técnico para Analista de Qualidade de Software Júnior**.

O objetivo deste desafio é demonstrar a capacidade de **analisar um sistema sem documentação formal de requisitos**, identificar funcionalidades, modelar cenários de teste, executar testes e registrar defeitos de forma clara e organizada.

---

# Aplicação analisada

Aplicação disponibilizada para o desafio:

https://creative-sherbet-a51eac.netlify.app/

A aplicação consiste em um sistema simples de **gerenciamento de cursos**, permitindo que usuários realizem operações básicas sobre cursos cadastrados.

---

# Objetivo da aplicação

Com base na exploração da interface e no comportamento observado durante o uso do sistema, é possível inferir que o objetivo da aplicação é permitir o **gerenciamento de cursos**, possibilitando que usuários:

- Cadastrem novos cursos
- Visualizem cursos cadastrados
- Excluam cursos existentes

Dessa forma, a aplicação funciona como um **módulo simples de administração de cursos**, com foco nas operações básicas de cadastro e gerenciamento.

---

# Análise exploratória do sistema

A aplicação foi analisada utilizando uma abordagem de **exploração funcional**, considerando que não há documentação formal de requisitos disponível.

A partir da navegação na interface e da execução das funcionalidades disponíveis, foi possível identificar os **principais fluxos do sistema**.

---

# Funcionalidades identificadas

Durante a exploração da aplicação foram identificados **três fluxos principais**:

## 1. Cadastro de cursos

Fluxo responsável por permitir que o usuário registre um novo curso no sistema.

O processo envolve o preenchimento de um formulário contendo informações do curso, como por exemplo:

- Nome do curso
- Descrição
- Instrutor
- Data de início
- Data de término
- Número de vagas
- Tipo de curso
- URL da imagem
- Campos adicionais dependendo do tipo de curso

Após o preenchimento do formulário, o usuário pode confirmar o cadastro.

Comportamento esperado:

- O sistema deve validar os campos necessários
- O curso deve ser registrado com sucesso
- O curso deve aparecer na listagem após o cadastro

---

## 2. Listagem de cursos

Fluxo responsável por exibir todos os cursos cadastrados no sistema.

A listagem permite visualizar informações importantes de cada curso e possibilita a interação com os cursos já cadastrados.

Comportamento esperado:

- Todos os cursos cadastrados devem ser exibidos
- As informações do curso devem ser apresentadas corretamente
- A lista deve refletir alterações realizadas no sistema (cadastro ou exclusão)

---

## 3. Exclusão de cursos

Fluxo responsável por permitir a remoção de cursos cadastrados.

O usuário pode excluir um curso diretamente a partir da listagem.

Comportamento esperado:

- O curso selecionado deve ser removido da lista
- A interface deve atualizar corretamente após a exclusão

---

# Pontos críticos para teste

Com base na análise da aplicação, alguns pontos foram considerados críticos para garantir o correto funcionamento do sistema:

### Validação de campos do formulário
Garantir que os campos aceitem apenas valores válidos e que campos obrigatórios sejam corretamente tratados.

### Regras de negócio relacionadas ao cadastro
Verificar consistência das informações inseridas, como por exemplo:

- coerência entre datas
- formato de URLs
- valores válidos para número de vagas

### Integridade da listagem
Garantir que os cursos cadastrados sejam exibidos corretamente e que a listagem reflita alterações realizadas no sistema.

### Exclusão de cursos
Garantir que cursos possam ser removidos corretamente e que a interface seja atualizada após a exclusão.

### Comportamentos inesperados
Testar o sistema com entradas inválidas ou cenários não previstos para verificar a robustez da aplicação.

---

# Estratégia de modelagem de testes

Como não há documentação formal de requisitos, a modelagem de testes foi baseada no **comportamento observado do sistema**.

A estratégia adotada seguiu três etapas principais:

1. **Identificação das funcionalidades do sistema**
2. **Criação de cenários de teste**
3. **Detalhamento em casos de teste executáveis**

Essa abordagem permite transformar a análise exploratória em um conjunto estruturado de testes.

---

# Cenários de teste

Os cenários de teste representam **situações ou comportamentos que precisam ser validados no sistema**.

Eles foram definidos com base nos fluxos identificados:

- Cadastro de cursos
- Listagem de cursos
- Exclusão de cursos

Os cenários cobrem diferentes tipos de teste, incluindo:

- cenários positivos
- cenários negativos
- validações de campos
- comportamentos inesperados

---

# Casos de teste e execução

Cada cenário foi detalhado em **casos de teste**, contendo:

- pré-condições
- passos de execução
- resultado esperado

Após a criação dos casos de teste, foi realizada a **execução manual dos testes**, registrando:

- resultado obtido
- status do teste (PASS ou FAIL)
- evidẽncias

---

# Test Summary Report

Este relatório resume os resultados da execução dos testes realizados na aplicação de cadastro e gerenciamento de cursos.

Os testes foram executados manualmente com base nos cenários e casos de teste definidos durante a fase de análise do sistema.

---

## Visão Geral da Execução dos Testes

| Métrica | Quantidade |
|--------|-----------|
| Total de cenários de teste | 13 |
| Total de casos de teste | 19 |
| Casos de teste executados | 19 |
| Testes aprovados (PASS) | 08 |
| Testes reprovados (FAIL) | 11 |
| Bugs identificados | 11 |


---

## Cobertura por Funcionalidade

| Funcionalidade | Casos de teste |
|---------------|---------------|
| Cadastro de cursos | 13 |
| Listagem de cursos | 05 |
| Exclusão de cursos | 01 |

---

## Análise dos Resultados

A execução dos testes permitiu validar os principais fluxos da aplicação, incluindo cadastro, listagem e exclusão de cursos.

Os testes cobriram cenários positivos, negativos e validações de comportamento do sistema.

Durante a execução foram identificados alguns comportamentos inesperados, que foram registrados e detalhados na seção de **registro de bugs** deste repositório.

---


# Registro de bugs

Durante a execução dos testes, comportamentos inconsistentes ou inesperados foram registrados como **bugs**.

Cada bug documentado contém:

- título do problema
- passos para reprodução
- resultado atual
- resultado esperado
- severidade ou impacto

Essa documentação permite que os defeitos sejam compreendidos e reproduzidos com facilidade.

---

# Documentação dos testes

A documentação completa dos testes está disponível na planilha abaixo:

📄 Planilha de testes  


A planilha está organizada em **três abas**:

### Cenários
Contém os cenários de teste identificados durante a análise da aplicação.

### Casos de teste / Execução
Contém os casos de teste detalhados, bem como o resultado da execução de cada teste.

### Bugs
Contém o registro dos problemas encontrados durante a execução dos testes.

---

# Evidências da execução dos testes

As evidências da execução dos testes (prints ou gravações de tela) estão disponíveis no link abaixo:

📂 Evidências dos testes 

https://jam.dev/s/1244af56-0a28-4c7d-b78f-fb0310a6e650/xscp

---

# Ferramentas utilizadas

Durante a realização do desafio foram utilizadas as seguintes ferramentas:

- **Google Sheets** — documentação dos cenários, casos de teste e execução
- **Jam.Dev** — captura e armazenamento de evidências
- **Chrome Web Browser** — execução manual dos testes

---

# Considerações finais

Este desafio permitiu aplicar práticas fundamentais de **Quality Assurance**, incluindo:

- análise exploratória de sistemas
- identificação de funcionalidades sem documentação de requisitos
- modelagem de cenários de teste
- criação e execução de casos de teste
- registro estruturado de bugs

