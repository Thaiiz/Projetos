# 📌 Automação de Processo – Desafio

## 📖 Descrição do Projeto

Este projeto tem como objetivo automatizar o processo de:

* Acesso ao sistema da empresa
* Download da base de dados
* Cálculo de indicadores
* Envio automático de e-mail com os resultados

A automação é feita utilizando Python.

# 🚀 Passo a Passo do Desafio

## 1️⃣ Entrar no sistema da empresa

* Abrir o Google Chrome
* Digitar o link do sistema (Drive da empresa)
* Apertar **Enter** e aguardar carregamento

## 2️⃣ Navegar no sistema

* Localizar a base de dados
* Acessar a página de exportação

## 3️⃣ Exportar a base de dados

* Realizar o download do arquivo
* Salvar em diretório local

## 4️⃣ Calcular os Indicadores

* 📊 **Faturamento total**
* 📦 **Quantidade de produtos vendidos**

## 5️⃣ Enviar as informações por e-mail

* Gerar resumo com os indicadores
* Enviar automaticamente para o responsável

---

# 🛠️ Tecnologias Utilizadas

* Python 3
* PyAutoGUI (automação)
* OpenPyXL (manipulação de planilhas)
* Python-dotenv (variáveis de ambiente)

---

# 📦 Instalação das Dependências

Execute os seguintes comandos:

```bash
pip install pyautogui
pip install openpyxl
pip install python-dotenv
```

---

# ⚙️ Configurações Importantes

### ⏱ Pausa entre comandos

```python
pyautogui.PAUSE = 0.5
```

Define uma pausa automática entre cada comando.

---

### 🕒 Espera após último comando

```python
import time
time.sleep(0.5)
```

Usado para aguardar carregamentos ou finalizações.

---

# 🔐 Variáveis Sensíveis

Utilize o `python-dotenv` para armazenar:

* Email
* Senha
* Caminhos importantes
* Links privados

Exemplo `.env`:

```
EMAIL=seuemail@email.com
SENHA=sua_senha
```

---

# 📊 Indicadores Calculados

O sistema calcula automaticamente:

* ✅ Faturamento total
* ✅ Quantidade total de produtos vendidos

---

# 📧 Resultado Final

Ao final da execução, o sistema:

* Baixa os dados
* Calcula os indicadores
* Envia um e-mail automático com os resultados
