# ⚓ Sistema de Criptografia da Guarda Costeira

Este é um sistema simples de **Criptografia e Descriptografia** desenvolvido em **Python** para uso interno da Guarda Costeira.  
Ele utiliza o algoritmo **AES (Advanced Encryption Standard)** no modo **ECB (Electronic Codebook)**, usando a **senha do inspetor logado como chave de criptografia**.

---

## 🔑 Funcionalidades Principais

- **Autenticação Restrita**  
  Acesso apenas para inspetores pré-registrados (limite de **3 tentativas**).  
  A **senha do inspetor** funciona como **chave secreta** para criptografar/descriptografar.

- **Criptografia AES-128**  
  Como a senha é um **hexadecimal de 16 bytes (32 caracteres)**, o sistema utiliza AES-128.

- **Descriptografia**  
  Mensagens podem ser decodificadas usando a mesma chave do inspetor.

- **Codificação Base64**  
  Facilita envio e armazenamento das mensagens criptografadas.

- **Controle de Tamanho**  
  Mensagens para criptografia são limitadas a **128 caracteres**.

---

## ⚙️ Pré-requisitos

Certifique-se de ter o **Python** instalado.

### 📦 Bibliotecas Necessárias

- `pycryptodome` — para criptografia AES  
- `base64` — biblioteca nativa do Python

### Instalação

```bash
pip install pycryptodome
