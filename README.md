# 📦 SGV - Sistema Gerenciador de Vendas & Estoque

![Java](https://img.shields.io/badge/Java-17-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![H2 Database](https://img.shields.io/badge/H2_Database-003545?style=for-the-badge&logo=database&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)

## 📌 Sobre o Projeto

O **SGV (Sistema Gerenciador de Vendas)** é uma aplicação web desenvolvida como projeto prático para aprofundamento em **Programação Orientada a Objetos (POO)** em Java. 

O objetivo do sistema é simular um ambiente real de gestão, permitindo o controle de acesso de usuários e a administração de dados através de uma interface web, conectada a um banco de dados em memória.

### 🚀 Principais Aprendizados e Funcionalidades
* Aplicação prática de conceitos de POO (Encapsulamento, Herança, Polimorfismo).
* Gerenciamento de dependências e build com Maven.
* Configuração e integração com banco de dados em memória (H2 Database).
* Criptografia e autenticação de senhas (Hash).
* Criação de interface web interativa (HTML/CSS) servida pelo backend Java.

---

## 🛠️ Tecnologias Utilizadas

* **Backend:** Java 17
* **Frontend:** HTML5
* **Banco de Dados:** H2 Database Engine (In-memory)
* **Gerenciador de Dependências:** Maven

---

## ⚙️ Como executar o projeto localmente

Siga as instruções abaixo para configurar e rodar o projeto na sua máquina.

### Pré-requisitos
Certifique-se de ter instalado em sua máquina:
* [JDK 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html) (Oracle ou OpenJDK)
* Uma IDE de sua preferência (NetBeans, IntelliJ IDEA ou Eclipse)
* Git

### Passo a Passo

**1. Clone o repositório**
`git clone https://github.com/TheoGuerra71/inventory-service.git`

**2. Compile e execute o projeto**
Abra o projeto na sua IDE, clique com o botão direito sobre a raiz do projeto e selecione **"Build Project"** (ou use o Maven diretamente). Em seguida, clique em **"Run"**.

**3. Configure o Banco de Dados (Criação do Admin)**
Com a aplicação rodando, precisamos criar o usuário administrador no banco de dados H2.
* Abra o navegador e acesse o console do banco: `https://localhost:8443/h2-console`
* Preencha os dados de conexão:
  * **JDBC URL:** `jdbc:h2:~/db`
  * **User Name:** `sgv`
  * **Password:** `123`
* Conecte-se e execute o seguinte script SQL para inserir o usuário admin:

```sql
INSERT INTO Usuario (login, senha, papel, id) VALUES 
('admin', '$2a$10$K6PG.YUsSpMT/LOyPpeB5eUVdPlmfDfSH.N0xLHAC1NbgblBhraHe', 'ADMIN', 1);
Clique no botão Run (Verde).

4. Acesse a Aplicação
Agora que o banco está configurado, acesse o sistema pelo navegador:

URL: https://localhost:8443/

Login: admin

Senha: 123

Pronto! O sistema está configurado e pronto para uso.
