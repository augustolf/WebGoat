# LEIAME

## Sobre o Projeto

O **WebGoat** é uma aplicação web propositalmente vulnerável, desenvolvida para fins educacionais e de treinamento em segurança da informação. Inspirado pelo projeto OWASP, o WebGoat permite que desenvolvedores, testadores e profissionais de segurança pratiquem técnicas de ataque e defesa em um ambiente seguro e controlado.

## Funcionalidades
- Diversas lições práticas sobre vulnerabilidades comuns (OWASP Top 10)
- Interface web intuitiva e interativa
- Exercícios guiados para aprendizado prático
- Suporte a múltiplos idiomas
- Integração com ferramentas de análise de segurança

## Aviso de Segurança
> **Atenção:** Nunca utilize o WebGoat em ambientes de produção. Ele é destinado exclusivamente para fins educacionais e de pesquisa. Ao rodar esta aplicação, sua máquina estará vulnerável a ataques.

## Pré-requisitos
- Java 11 ou superior
- Maven 3.6+
- Docker (opcional)

## Instalação

### 1. Clonando o repositório
```bash
git clone https://github.com/augustolf/WebGoat.git
cd WebGoat
```

### 2. Compilando o projeto
```bash
./mvnw clean install
```
No Windows, use `mvnw.cmd`.

### 3. Executando com Maven
```bash
./mvnw spring-boot:run
```

### 4. Executando com Docker (opcional)
```bash
docker build -t webgoat .
docker run -p 8080:8080 webgoat
```

## Como Usar
Após iniciar a aplicação, acesse:

    http://localhost:8080/WebGoat

- Faça login com as credenciais padrão (se necessário)
- Navegue pelas lições e siga as instruções para aprender sobre cada vulnerabilidade

## Estrutura do Projeto
```
WebGoat/
├── src/                  # Código-fonte e recursos
├── config/               # Configurações e scripts auxiliares
├── docs/                 # Documentação e imagens
├── Dockerfile            # Build para container Docker
├── pom.xml               # Configuração do Maven
└── LEIAME.md             # Este arquivo
```

## Contribuição
Contribuições são bem-vindas! Para contribuir:
1. Faça um fork deste repositório
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas alterações (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

Consulte o arquivo [CONTRIBUTING.md](CONTRIBUTING.md) para mais detalhes.

## Licença
Este projeto está licenciado sob a licença [MIT](LICENSE.txt).

## Referências
- [OWASP WebGoat (site oficial)](https://owasp.org/www-project-webgoat/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [Documentação do projeto](docs/README.md)
