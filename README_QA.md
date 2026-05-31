# Portfólio de Testes e Garantia de Qualidade (QA)
    
Olá! Meu nome é **Nataly Santos**. Tenho ampla experiência profissional em auditoria operacional e controle de conformidade (Cinépolis), além de sólida formação prática em lógica de programação, **Python**, banco de dados (**SQLite/PostgreSQL**), APIs REST, gerenciamento de dados com **Power BI** e desenvolvimento ágil.

Este repositório consolida o meu portfólio prático de QA pronto para o mercado, detalhando as evidências de minha mentalidade de prevenção a riscos e rigor técnico.

---

## 🛠️ Habilidades Técnicas (My Toolkit)
- **Metodologias de Teste**: Testes Manuais, Cenários Funcionais, Teste de Regressão, Teste Exploratório, Caixa Preta.
- **Estruturação de Artefatos**: Casos de Teste (Test Cases), Planos de Teste e Relatórios de Bug (Bug Reports) de alta severidade.
- **Testes de API**: Validações de endpoints e códigos de retorno HTTP (200, 201, 400, 404, 500) usando **Postman**.
- **Segurança de Bancos**: Atuação com consultas estruturadas SQL (**SELECT, JOINs, GROUP BY, aggregates**).
- **Processos de Engenharia**: Cultura Ágil (**Scrum, Kanban**) e ciclo de vida de tickets no **Jira**.
- **Automação (Diferencial)**: Scripts de automação funcional de interface web utilizando **Selenium-Python webdriver**.

---

## 📂 Projetos Simulados & Práticos

### 1. Modelagem de Casos de Teste (Test Case)
- **ID**: `TC01_COMPRA_MEIA_ESTUDANTE`
- **Cenário**: Validar a compra de ingresso online com a modalidade "Meia-Entrada Estudante" utilizando dados de cartão válidos.
- **Passos para reprodução**:
  1. Acessar site e escolher um filme ativo comercialmente.
  2. Selecionar o assento de escolha no mapa interativo.
  3. Clicar no tipo de entrada "Meia Estudante" do catálogo e preencher o código da carteirinha.
  4. Preencher o cartão financeiro de crédito válido.
  5. Acionar o botão "Finalizar Compra".
- **Resultado Esperado**: O sistema processa o pagamento via integração gateway, gera um QR Code oficial do bilhete e altera o status na tabela do banco de dados relacional para "CONFIRMADO".

### 2. Bug Report de Elevado Rigor Técnico
- **Título**: `BUG: Botão de pagamento do aplicativo trava em tela escura ao processar tickets Meia-Entrada`
- **Severidade**: Alta | **Prioridade**: Alta
- **Passos**: 
  1. Acessar tela de check-out com ingresso de estudante.
  2. Clicar em "Prosseguir para Pagamento".
- **Resultado Esperado**: Exibição da tela operacional de preenchimento.
- **Resultado Obtido**: Aplicativo trava instantaneamente com HTTP 500.

### 3. Automação Funcional com Python & Selenium
\`\`\`python
from selenium import webdriver

# 1. Configurando driver
driver = webdriver.Chrome()

# 2. Navegando para o portal de vendas Cinépolis
driver.get("https://cinepolis.com/login")

# 3. Localizando os campos de formulário e submetendo
email = driver.find_element(by="id", value="email")
email.send_keys("nataly.qa@cine.com")

button = driver.find_element(by="id", value="btn-login")
button.click()

# 4. Validando resultado esperado assertivo
assert "Painel de Ingresso" in driver.title
driver.quit()
\`\`\`

---

## 📞 Contato
Vamos construir um software robusto juntos?
- **Email**: naity.santos2010@outlook.com
- **LinkedIn**: www.linkedin.com/in/nataly-beatriz-santos-reimers-4a8767242

