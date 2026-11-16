# BM Carretas Náuticas — site

Site da BM Carretas Náuticas: catálogo com preços, fotos, visualizador 3D/360°, configurador, simulador de financiamento, orçamento com protocolo, área do cliente e painel do administrador.

- Site estático em um único arquivo: `index.html` (publicado pelo GitHub Pages).
- Login e dados (orçamentos, preços, fotos) no Firebase: Authentication (e-mail/senha) + Cloud Firestore.
- Regras de segurança do banco em `firestore.rules`.

## Configuração
Tudo fica no bloco `CONFIG` no início do script do `index.html`:
- `whatsapp`, `email`, `endereco`: contatos da BM.
- `firebase`: configuração web do projeto Firebase.
- `adminEmails`: admin principal (o mesmo de `isMaster()` em `firestore.rules`). Outros admins são cadastrados no painel, aba Equipe.

## Painel do administrador
Ícone de pessoa no topo → aba **Administrador**. Menu lateral: Visão geral, Orçamentos, Clientes, Fluxo de caixa, Receitas, Despesas, Produtos e preços, Fotos e Equipe e acessos.
