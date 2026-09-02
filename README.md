# 🧪 Manual Testing Project: LinkedIn Login Page

This project demonstrates my practical skills in Manual QA, focusing on test scenario design, execution, and bug documentation.

## 📋 Test Cases (Casos de Teste)

### 🔑 Scenario 1: Successful Login with Valid Credentials
*   **Pre-conditions:** User must have a registered account.
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Enter a valid email address in the "Email" field.
    3. Enter the correct password in the "Password" field.
    4. Click the "Sign in" button.
*   **Expected Result:** The user is successfully redirected to their LinkedIn Feed home page.
*   **Status:** ✅ PASSED

### ❌ Scenario 2: Login Failure with Incorrect Password
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Enter a valid email address.
    3. Enter an incorrect password.
    4. Click the "Sign in" button.
*   **Expected Result:** An error message appears stating "Wrong password" or "Invalid credentials", and the user remains on the login page.
*   **Status:** ✅ PASSED

### ⚠️ Scenario 3: Login Failure with Empty Fields
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Leave both "Email" and "Password" fields blank.
    3. Click the "Sign in" button.
*   **Expected Result:** Inline validation errors appear alerting the user that the fields are required.
*   **Status:** ❌ FAILED (Example Bug)


### 📋 Projeto 2: Testes de Automação / Manuais (Login)

| ID | Cenário de Teste | Passos para Executar | Resultado Esperado | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC-001** | Login com credenciais válidas | Introduzir e-mail e password corretos. Clicar em Entrar. | O utilizador entra na dashboard com sucesso. | **Pass** |
| **TC-002** | Login com password errada | Introduzir e-mail correto e password errada. Clicar em Entrar. | Mensagem de erro: "Password incorreta". O login é bloqueado. | **Pass** |
| **TC-003** | Login com campos vazios | Deixar e-mail e password em branco. Clicar em Entrar. | Mensagem de erro a pedir para preencher os campos obrigatórios. | **Pass** |
| **TC-004** | Login com formato de e-mail inválido | Escrever "utilizador123" (sem @) e password. Clicar em Entrar. | O sistema avisa que o e-mail não é válido antes de enviar o formulário. | **Pass** |
| **TC-005** | Recuperação de password | Clicar em "Esqueci-me da password", inserir e-mail válido. | Envio de e-mail com link de redefinição com sucesso. | **Pass** |



### 🛒 Projeto 3: Testes de Carrinho de Compras (E-commerce)

| ID | Cenário de Teste | Passos para Executar | Resultado Esperado | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC-006** | Adicionar produto ao carrinho | Clicar num produto e carregar no botão "Adicionar ao Carrinho". | O produto é adicionado e o contador do carrinho muda de 0 para 1. | **Pass** |
| **TC-007** | Alterar quantidade do produto | Entrar no carrinho e alterar a quantidade de 1 para 2 unidades. | O preço total do carrinho duplica e atualiza automaticamente. | **Pass** |
| **TC-008** | Remover produto do carrinho | Clicar no botão "Remover" ou no ícone do caixote do lixo. | O produto desaparece e mostra a mensagem "O seu carrinho está vazio". | **Pass** |
| **TC-009** | Limite de stock | Tentar adicionar 99 unidades de um produto com apenas 5 em stock. | O sistema mostra o aviso: "Não é possível adicionar por falta de stock". | **Pass** |
