# Teste

Página temporária feita para testar algumas funcionalidades do mkdocs. Em breve ela será removida do site.

## Testando o terminal

<div class="termy">

```console
$ pip install fastapi

---> 100%
```

</div>

## Testando código

Lista de passos:

* Passo 1
* Passo 2
* Passo 3

Crie um arquivo chamado `teste.py` e digite:

```Python
from typing import Union

from fastapi import FastAPI

app = FastAPI()


@app.get("/")
def read_root():
    return {"Hello": "World"}


@app.get("/items/{item_id}")
def read_item(item_id: int, q: Union[str, None] = None):
    return {"item_id": item_id, "q": q}
```

## Testando Admonition

??? note "Clique aqui"
    aaa  
    bbb  
    ccc
    
## Line highlight

```Python hl_lines="9  13-15"
from typing import Union

from fastapi import FastAPI

app = FastAPI()


@app.get("/")
async def read_root():
    return {"Hello": "World"}


@app.get("/items/{item_id}")
async def read_item(item_id: int, q: Union[str, None] = None):
    return {"item_id": item_id, "q": q}
```
