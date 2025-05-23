# Projeto: Sistema de Cadastro e Lista de Voluntários

Este projeto é uma aplicação web simples desenvolvida em HTML, CSS e JavaScript que permite o cadastro de voluntários, preenchimento automático de endereço via CEP, listagem dos usuários cadastrados, e redirecionamento automático após inatividade.

## 🔐 Acesso Inicial

**O uso do sistema deve começar pela página de login (`login.html`)**.  
A navegação correta garante o funcionamento do controle de sessão e redirecionamento por inatividade.

- Email: usuario@mail.com
- Senha: senha123

---

## 🔧 Funcionalidades

- Cadastro de usuários com validação de campos.
- Preenchimento automático do endereço via API do ViaCEP.
- Armazenamento dos usuários no `localStorage` do navegador.
- Listagem dos voluntários cadastrados com imagens aleatórias.
- Remoção de usuários da lista.
- Redirecionamento automático para a tela de login após 5 minutos de inatividade.

## 🚀 Como executar

1. **Clone ou copie os arquivos para sua máquina**  
   Certifique-se de ter todos os arquivos HTML, CSS e JS necessários.

2. **Inicie o sistema pela página de login**  
   Abra `login.html` em um navegador moderno (Chrome ou Firefox).  
   Exemplo:  
   `file:///C:/caminho/para/seu/projeto/login.html`

3. **Após o login, vá para a tela de cadastro**  
   Acesse `cadastrousuario.html` para cadastrar novos voluntários.

4. **Preencha os dados no formulário de cadastro**
   - Nome (mínimo 3 caracteres)
   - E-mail (mínimo 7 caracteres antes do `@` e 5 depois)
   - CEP (somente números, 8 dígitos)

   O endereço, bairro, cidade e estado serão preenchidos automaticamente usando a [API do ViaCEP](https://viacep.com.br).

5. **Ver a lista de voluntários**  
   Após o cadastro, acesse `listavoluntarios.html` para visualizar os voluntários registrados. As imagens são geradas automaticamente.

6. **Inatividade**  
   Após 5 minutos sem interações (cliques, teclas, rolagem, etc), o usuário será automaticamente redirecionado para `login.html`.

## 📁 Estrutura básica dos arquivos

meu-projeto/
│
├── login.html               # Página de login (início obrigatório)
├── cadastrousuario.html     # Página de cadastro de voluntários
├── listavoluntarios.html    # Página de listagem dos voluntários
├── style.css                # Estilos da interface
└── README.md                # Este arquivo com instruções

## 🔒 Observação

Os dados dos voluntários são armazenados localmente no navegador usando `localStorage`. Isso significa que:

- Os dados são perdidos se o usuário limpar os dados do navegador.
- Não há persistência em servidor — apenas local.

## 💡 Futuras melhorias sugeridas

- Autenticação real com senha e login.
- Backend com banco de dados.
- Upload de fotos reais dos usuários.
- Filtro e ordenação da lista de voluntários.

---

Desenvolvido com ❤️ para fins educacionais.
