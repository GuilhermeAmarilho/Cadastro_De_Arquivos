# 📄 Sistema de Upload com Sessão, Cookie e Geração de PDF (FPDF)

Este projeto em PHP implementa um sistema de login com controle por sessão e cookie, upload de arquivos por usuário autenticado, listagem dos arquivos enviados e geração de **relatório em PDF** utilizando a biblioteca **FPDF**.

Desenvolvido como prática no Ensino Médio Técnico, o projeto abrange múltiplos conceitos fundamentais do desenvolvimento web com PHP.

---

## 👨‍💻 Autor
- Guilherme Pereira do Amarilho
🎓 Ensino Médio Técnico
📅 Ano de criação: 2016
✉️ guiamarilho1@gmail.com
🔗 GitHub: @guilhermeamarilho

---

## 🧠 Tecnologias Usadas
- PHP (procedural)
- HTML5 / CSS3
- Cookies e Sessões
- Manipulação de arquivos via $_FILES
- Geração de PDF com FPDF

---

## 🧩 Funcionalidades

- 🔐 **Login com nome e email**
  - Criação de sessão
  - Nome salvo via **cookie com expiração de 5 minutos**
- 📁 **Upload de arquivos**
  - Arquivos enviados são armazenados por sessão
- 📂 **Listagem em tabela**
  - Exibe nome e tamanho dos arquivos enviados
- 🧾 **Geração de relatório em PDF** (via FPDF)
- 🚪 **Logout**
  - Encerra sessão e confirma destruição via `isset($_SESSION)`

---

## 📷 Telas do Sistema
- Login
    - Nome e email
    - Criação de sessão e cookie
- Formulário de Upload
    - Envio de arquivos
- Lista de Arquivos
    - Tabela com nome e tamanho
    - Botão para gerar relatório PDF
- PDF
    - Relatório com nome, email e arquivos enviados
- Logout
    - Destroi sessão e informa status

## 🚀 Como Executar
- Extraia o conteúdo do projeto em um servidor local com PHP (XAMPP, Laragon etc.)
- Extraia o fpdf.rar na raiz ou dentro de /arquivos para habilitar a geração de PDF
- Crie as pastas necessárias com permissão de escrita (ex: /uploads)
- Acesse pelo navegador:
    - http://localhost/seu-projeto/sessao/login.php

---

## 🗂️ Estrutura do Projeto

```text
.
├── index.html
    # Página inicial (opcional)
├── index.php
    # Geração de PDF com FPDF
├── sair.php
    # Logout e encerramento de sessão
├── enunciado.txt
    # Enunciado da atividade
├── fpdf.rar
    # Arquivos da biblioteca FPDF compactados
├── arquivos/
│   ├── envio.php
        # Script para processar upload
│   ├── form.php
        # Formulário de envio de arquivos
│   ├── fpdf.php
        # Relatório em PDF - versão 1
│   ├── fpdf2.php
        # Relatório em PDF - versão 2 (alternativa)
│   └── lista.php
        # Lista de arquivos enviados
├── css/
│   └── style.css
        # Estilo global
├── sessao/
│   ├── cadastro.php
        # Cadastro de usuário (opcional)
│   ├── login.php
        # Tela de login (nome e email)
│   ├── log.php
        # Registro de login
│   ├── sessao.php
        # Logout / verificação de sessão
│   ├── dados.txt
        # Armazena dados dos usuários (se usado)
│   └── css/
│       ├── style.css
│       ├── style1.css
│       └── style2.css
```