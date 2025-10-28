# PIT-LIVROS# Catálogo Simples de Livros 📚

Projeto desenvolvido em **Java (Servlet + JSP + JDBC)** como parte de um **Projeto Integrador Interdisciplinar** do curso de **Ciência da Computação**.

---

## 🚀 Tecnologias
- Java 17+
- Jakarta Servlet / JSP
- MySQL
- JDBC com `PreparedStatement` (para segurança contra SQL Injection)
- Tomcat 10+

---

## 🧱 Estrutura
```
src/
 ├── model/Livro.java
 ├── dao/ConnectionFactory.java
 ├── dao/LivroDAO.java
 └── servlet/LivroServlet.java
webapp/
 ├── index.jsp
 ├── formulario.jsp
 ├── listar.jsp
 ├── buscar.jsp
 ├── resultadoBusca.jsp
 └── styles.css
sql/
 └── schema.sql
```

---

## ⚙️ Configuração

1. Crie o banco de dados executando `sql/schema.sql` no MySQL.
2. Ajuste `USER` e `PASS` em `ConnectionFactory.java` com suas credenciais.
3. Compile e rode o projeto em um servidor **Tomcat**.
4. Acesse: [http://localhost:8080/catalogo_livros](http://localhost:8080/catalogo_livros)

---

## 🔒 Segurança
Todas as consultas SQL usam `PreparedStatement`, o que impede ataques de **SQL Injection**.
Os parâmetros são tratados como dados, nunca como parte do código SQL.

---

## 📚 Funcionalidades
- Adicionar livros ao catálogo
- Editar e remover livros
- Buscar por título ou autor (consulta segura)
- Interface simples em JSP

---

## 👨‍💻 Autor
Projeto criado como exemplo para atividades acadêmicas de modelagem e segurança em banco de dados.
```
Aluno: [Seu Nome Aqui]
Curso: Ciência da Computação
Disciplina: Projeto Integrador Interdisciplinar
```

---

## 📝 Licença
Uso acadêmico e educacional.
