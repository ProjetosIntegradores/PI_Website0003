# Pi_Website0003
Site aplicativo do Projeto Integrador 3 na Univesp  
Cliente: TekTintas

### Página Inicial

* [Página do PI1](https://github.com/ProjetosIntegradores/Pi_Website0001)

* [Página do Render](https://gestao-pi-render.onrender.com/)

## Participantes do Projeto
```
GABRIEL ANTONIO RIBEIRO DA SILVA
LUCAS EDSON SANTOS SILVA
BRUNO ROSENDO ALVES
SILVIO SOARES PEREIRA
```

## História e Desenvolvimento

O código do Projeto Integrador 3 foi desenvolvido no Visual Studio Code, utilizando Python e Django. Meu computador trava toda vez que tento virtualizar máquinas em Linux ou usar Docker Desktop.

Depois de muito esforço, consegui criar um site com banco de dados. Enfrentei diversas dificuldades durante o desenvolvimento, mas, com a ajuda de vídeos no YouTube*, repositórios do GitHub** e cursos da faculdade***, consegui criar um banco de dados funcional. Porém, isso só foi suficiente para o PI1. O PHP tinha péssima integração com outras ferramentas (pelo menos da maneira que eu tinha feito) e meu computador é incompatível.

A princípio, comecei usando Python, mas depois de falhar algumas vezes tentando fazer sozinho (por dois meses sem usar IA), sem instruções, troquei para PHP para melhor seguir as instruções de outros desenvolvedores. Até perceber que o site desenvolvido não cumpria os requisitos do PI3. Resolvi voltar para Python e Django, dessa vez com ajuda de IAs como Copilot e Gemini.

**Solução para o cliente:** criar um website que promovesse a loja e um aplicativo onde os usuários pudessem cadastrar suas informações para futuras promoções e contatos.

**Objetivo do projeto:** desenvolver um software com framework web ou aplicativo que utilize banco de dados, inclua script web (JavaScript), nuvem, controle de versão, acessibilidade, integração contínua, testes e análise de dados.

A parte do PI1 foi suficiente para o banco de dados e script web (JavaScript), porém o restante apresentou muitos problemas que não consegui resolver com PHP. Por isso, recomecei o projeto usando Python. Este website no Render (gestao_pi_render) possui uma tabela dinâmica que exibe informações sobre quantos clientes foram inscritos na base de dados em determinado período. O site está hospedado na nuvem (Render), utiliza banco de dados PostgreSQL, JavaScript para a tabela, controle de versão, testes e integração contínua, atendendo assim aos requisitos do projeto.

## Instalação e Configuração Local

1. **Clone o repositório:**
   ```
   git clone https://github.com/ProjetosIntegradores/PI_Website0003
   cd gestao_pi_render
   ```

2. **Crie e ative o ambiente virtual:**
   - No Windows (PowerShell):
     ```
     python -m venv venv
     .\venv\Scripts\Activate.ps1
     ```
   - No Linux/Mac:
     ```
     python3 -m venv venv
     source venv/bin/activate
     ```

3. **Instale as dependências:**
   ```
   pip install -r requirements.txt
   ```

4. **Configure as variáveis de ambiente:**
Na `.env` do projeto adicione:
     ```
     DJANGO_SECRET_KEY=sua_chave_secreta
     DJANGO_DEBUG=True
     DJANGO_ALLOWED_HOSTS=localhost,127.0.0.1
     ```

5. **Aplique as migrações do banco de dados:**
   ```
   python manage.py migrate
   ```

6. **Crie um superusuário (opcional, para acessar o admin):**
   ```
   python manage.py createsuperuser
   ```

7. **Inicie o servidor de desenvolvimento:**
   ```
   python manage.py runserver
   ```

8. **Acesse o site:**
   - Abra o navegador e vá para: [http://localhost:8000](http://localhost:8000)

## Referências e Citações
* Gustavo Neitzke, Sistema com Login, Cadastro, Sessões e Listagem de dados com CRUD  
  https://www.youtube.com/playlist?list=PLSHNk_yA5fNjoIRNHV-3FprsN3NWPcnnK  
* Lucas C. Achcar, Univesp PI_2  
  https://github.com/piunivespintegrador/pi2_univesp  
* UNIVESP, Eixo de Computação | Banco de Dados (2020.1)  
  https://www.youtube.com/playlist?list=PLxI8Can9yAHeZcEzZElhxwsQTf9MaG6sS