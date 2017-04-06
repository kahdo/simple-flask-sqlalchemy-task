# simple-flask-sqlalchemy-task
Tarefa:

Produção de uma pequena API web com apenas 1 método, "/getcities". Este método retornará uma lista de cidades armazenadas em um banco SQLite3 **que é acessado no Python via o framework SQLAlchemy**.

----


Premissas:

- Utilizar **Python 3.5**

- Utilizar um **VirtualEnv**:

    - Na raiz deste repositório você encontrará um arquivo de nome ```pip_requirements.txt```. Use este arquivo para instalar os frameworks necessários à execução da tarefa (Flask e SQLAlchemy)

        ```
        $ pip install -r pip_requirements.txt
        ```


- Utilizar o **SQLAlchemy** para definir uma tabela "Cities" no banco de dados com os seguintes campos:
    - **id**, chave primária, "id único da cidade"
    - **cityname**, "nome da cidade"
    - *OBS:* Cadastrar alguns dados nesse banco de dados, a fim de permitir o retorno pelo método de api.
    - *Bonus Points:* Não utilizar a construct Table() do SQLAlchemy manualmente, e sim definir a tabela por meio de uma classe Python que tem como herança direta uma [Base Declarativa do SQLAlchemy](http://docs.sqlalchemy.org/en/latest/orm/tutorial.html)

- Utilizar o **FLASK** para servir o conteúdo como um JSON ou lista básica:
    - Criar um método que possa ser retornado via HTTP.
    - Utilizar o próprio servidor web embutido do Flask (app.run())

----

- Entregável:

    - Aplicação Python que sirva um método http "/getcities" e que retorne uma lista das cidades que estão cadastradas no Banco de Dados, via os métodos do SQLAlchemy
    - Documentação *basica* de como rodar a sua solução.
    - Código completo em um repositório GIT **ou**, caso não consiga, uma pasta zipada mesmo.

- Metodologia do Teste:

    - Rodar a aplicação localmente:
        - Em sua execução inicial, a mesma irá criar o banco de dados, populando-o com alguns nomes de cidades.
        - Iniciar o servidor HTTP embutido no Flask
    - Abrir um navegador e digitar a url que o Flask aponta no console, ex.: http://127.0.0.1:8000/getcities e inspecionar se os dados são retornados.
    - Análise do código-fonte, estilo, pythonismos e etc.

----

Dicas:

- Manter um mínimo de organização, apenas o bom senso, sem exageros.
    - Exemplo: não entregar toda a aplicação em um único arquivo de código.

- *(Embora não seja obrigatório)* Gostaria de receber a tarefa em um repositório GIT, afinal esta é a ferramenta de versionamento de código que é usada no projeto real, e aí vou poder avaliar a sua proficiência no uso desta ferramenta.

- A sua capacidade de aprender, aplicar algo novo e se adaptar contará mais do que a quantidade de frameworks e tecnologias que você sabe hoje, pois o estudo de novas tecnologias é uma constante no projeto real.
    - Isso significa que, analisando o seu código, perguntarei sobre como e porquê você resolveu a task da maneira que você fez.
    - Entrelinhas: Copy-paste de pedaços/snippets de código da Internet não é pecado, e sim fonte de aprendizado genuína, mas eu preciso saber que você foi capaz de compreender e adaptar o que encontrou às suas necessidades, ou seja, se for por este caminnho, *documente suas referências* e assim poderei também avaliar a sua capacidade de caçar informação e ser ágil.

- Seja honesto no feedback se algo não der certo.


---

Tempo idealizado para execução da tarefa: **4 a 6 horas** *(já contando o desconhecimento do SQLAlchemy/Flask, ou seja, utilização de tutoriais/documentação das bibliotecas, pesquisas ao Stack Overflow, etc)* **:-D**

**OBS: Não há prazo para a tarefa, a estimativa acima é apenas para projetar o quanto um desenvolvedor junior em ambas as tecnologias flask/sqlalchemy mas com algum conhecimento de Python levaria em média para realizar esta task.**

Use o que for necessário para atingir o objetivo e documente os seus achados.



Obrigado! --Cadu