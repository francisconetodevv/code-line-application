# 🧰 Aplicação de Linha de Comando

Este é um projeto simples em Go que demonstra como criar uma aplicação de linha de comando utilizando a biblioteca [urfave/cli](https://github.com/urfave/cli). A aplicação permite buscar **IPs** e **servidores DNS (NS)** de um domínio informado.

---

## 📦 Sobre o Projeto

Esta ferramenta de linha de comando oferece dois comandos principais:

- `ip`: Realiza uma busca pelos IPs associados a um domínio.
- `servidores`: Retorna os nomes dos servidores DNS (Name Servers) do domínio.

---

## 🚀 Como Executar

### Pré-requisitos

- Go 1.22 ou superior instalado

### Clone o repositório

```bash
git clone https://github.com/francisconetodevv/code-line-application.git
cd code-line-application
```

### Instale as dependências

```bash
go mod tidy
```

### Execute o programa

```bash
go run main.go <comando> --host <domínio>
```

### Exemplos de uso

Buscar IPs de um domínio:

```bash
go run main.go ip --host devbook.com.br
```

Buscar servidores DNS de um domínio:

```bash
go run main.go servidores --host devbook.com.br
```

---

## 🛠 Estrutura do Projeto

```
code-line-application/
├── app/
│   └── app.go         # Lógica principal da aplicação CLI
├── main.go            # Ponto de entrada da aplicação
├── go.mod             # Dependências e configurações do Go
├── go.sum             # Hash das dependências
```

---

## 🧪 Bibliotecas Utilizadas

- [urfave/cli](https://github.com/urfave/cli) — Para criação e gerenciamento da CLI
- `net` (padrão do Go) — Para resolver IPs e servidores DNS

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT.

---

## ✍️ Autor

Desenvolvido por [José Francisco](https://github.com/francisconetodevv).
