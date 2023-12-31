# marvelapi

**Avengers API**

A Avengers API é uma API REST que permite a consulta de dados sobre os personagens da Marvel Comics. A API é escrita em Python e usa o Django como framework.

A API fornece os seguintes recursos:

* **Personagens:** Esta rota retorna uma lista de todos os personagens da Marvel Comics. Cada personagem é representado por um objeto JSON que contém as seguintes informações:
    * Nome
    * Sobrenome
    * Poderes
    * Equipamentos
    * Primeiros quadrinhos
    * Últimos quadrinhos
* **Quadrinhos:** Esta rota retorna uma lista de todos os quadrinhos da Marvel Comics. Cada quadrinho é representado por um objeto JSON que contém as seguintes informações:
    * Título
    * Número
    * Data de publicação
    * Escritor
    * Artista
    * Desenhista
* **Equipes:** Esta rota retorna uma lista de todas as equipes da Marvel Comics. Cada equipe é representada por um objeto JSON que contém as seguintes informações:
    * Nome
    * Membros
    * Primeiros quadrinhos
    * Últimos quadrinhos

A API também fornece as seguintes rotas:

* **/characters/search:** Esta rota permite a consulta de personagens por nome ou sobrenome.
* **/comics/search:** Esta rota permite a consulta de quadrinhos por título ou número.
* **/teams/search:** Esta rota permite a consulta de equipes por nome.

A API está disponível gratuitamente para uso pessoal e comercial. Para mais informações, visite o site da Avengers API.

**Instalação**

Para instalar a Avengers API, você precisará de uma instalação Python 3.6 ou superior. Depois de instalar o Python, você pode instalar a API usando o seguinte comando:

```
pip install avengers-api
```

**Uso**

Para usar a Avengers API, você precisará importar o módulo `avengers_api`. Depois de importar o módulo, você pode usar as funções e classes fornecidas para consultar dados sobre os personagens da Marvel Comics.

Por exemplo, para consultar a lista de todos os personagens, você pode usar o seguinte código:

```
from avengers_api import Characters

characters = Characters()

for character in characters:
    print(character)
```

Este código imprimirá a seguinte saída:


{
    "name": "Tony Stark",
    "last_name": "Stark",
    "powers": ["Genius", "Billionaire", "Playboy", "Philanthropist"],
    "equipment": ["Iron Man suit", "Jarvis AI"],
    "first_comics": ["Iron Man #1 (1968)"],
    "last_comics": ["Iron Man #700 (2012)"]
}

{
    "name": "Steve Rogers",
    "last_name": "Rogers",
    "powers": ["Superhuman strength", "Superhuman speed", "Superhuman agility", "Superhuman durability", "Superhuman healing factor"],
    "equipment": ["Captain America shield"],
    "first_comics": ["Captain America Comics #1 (1941)"],
    "last_comics": ["Captain America: Steve Rogers #54 (2017)"]
}

...
