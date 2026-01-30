# 🔐 Digital Envelope — Criptografia em Python

Este projeto consiste em uma implementação de um **Envelope Digital** em Python, utilizando a biblioteca **PyCryptodome**, com o objetivo de garantir a **confidencialidade** e a **integridade** de dados transmitidos eletronicamente.

Um envelope digital é uma técnica criptográfica que combina **criptografia simétrica** e **criptografia assimétrica**, permitindo proteger informações sensíveis durante a comunicação.

---

## 📌 Sobre o Projeto

O sistema simula a comunicação segura entre dois usuários:

- **Alice (Remetente)**
- **Bob (Destinatário)**

A mensagem é criptografada com um algoritmo simétrico, e a chave utilizada é protegida com criptografia assimétrica, formando o envelope digital.

O projeto foi desenvolvido com fins educacionais, visando a aplicação prática de conceitos estudados em sala de aula.

---

## 🛠️ Tecnologias Utilizadas

- Linguagem: Python
- Biblioteca: PyCryptodome
- Criptografia:
  - Simétrica (ex: AES)
  - Assimétrica (RSA)
- Codificação: Base64

---

## 📚 Referência

- [PyCryptodome — Documentação Oficial](https://pycryptodome.readthedocs.io/en/latest/)

---

## 📖 Aprendizados

Com este projeto, foi possível:

- Compreender o funcionamento do envelope digital
- Aplicar criptografia simétrica e assimétrica
- Implementar geração de chaves
- Trabalhar com arquivos criptografados
- Praticar segurança da informação em aplicações reais

Além disso, o projeto contribuiu para a consolidação de conceitos abstratos estudados na disciplina.

---

## ⚙️ Instalação

### Clone o repositório

```bash
git clone https://github.com/V1ntag3/digital-envelope.git
Acesse o diretório
cd digital-envelope
Instale a dependência
pip install pycryptodome
```
## 📁 Estrutura do Projeto
```bash
digital-envelope/
 ├── alice_sender/
 │   └── plaintext.txt
 ├── bob_receiver/
 ├── creation_of_asymmetric_keys.py
 ├── digital_envelope_creation.py
 └── open_digital_envelope.py
```
##📌 Orientações de Desenvolvimento
Cada diretório representa o ambiente da Alice (remetente) e do Bob (destinatário).
O script creation_of_asymmetric_keys.py gera novas chaves assimétricas.
Ao executá-lo, as chaves antigas são substituídas.
Será necessário gerar novamente o envelope.
O texto em claro pode ser editado em:
```bash
alice_sender/plaintext.txt
```
Os caminhos dos arquivos podem ser alterados via menu.
As entradas são feitas pelo teclado no console.
Basta digitar a abreviação do algoritmo (ex: aes).

## ▶️ Tutorial de Execução
### 1️⃣ Gerar Chaves (Opcional)
```bash
python creation_of_asymmetric_keys.py
```
### 2️⃣ Criar Envelope Digital
```bash
python digital_envelope_creation.py
```
Informe:
- Caminho do texto em claro
- Caminho da chave pública
- Algoritmo (ex: aes)

## 3️⃣ Abrir Envelope Digital
```bash
python open_digital_envelope.py
```
Informe:
- Caminho da mensagem criptografada
- Caminho da chave criptografada
- Caminho da chave privada
- Algoritmo utilizado

## 🔒 Funcionamento
- A mensagem é criptografada
- A chave é protegida com RSA
- Ambos são enviados juntos

O destinatário recupera a chave

A mensagem é descriptografada
