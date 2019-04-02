_forked from [samiraguiar](https://github.com/samiraguiar/docker-irpf)_

# Imagem Docker para o Programa IRPF (Imposto de Renda Pessoa Física)

Imposto de Renda Pessoa Física: [O que é?](http://receita.economia.gov.br/interface/cidadao/irpf)

Para executar:

```sh
docker run -ti --rm -e DISPLAY --net=host --pid=host --ipc=host irpf
```

Note que a montagem de volume (-v $HOME:/home/irpf) é opcional e pode ser alterada para outros diretórios caso desejado.

**Importante**: Este projeto é apenas uma prova de conceito e não substitui o programa oficial disponibilizado pela Receita Federal, além de não estar associado de forma alguma a este órgão. O autor não se responsabiliza por quaisquer erros na declaração e possíveis problemas com o Fisco causados pela utilização desta imagem.

Para realizar o build:
```sh
docker-compose build irpf
```

Para baixar e utilizar a imagem existente:
```sh
docker-compose pull
```

Primeira execução:
```sh
docker-compose run --name irpf irpf
```

Demais execuções:
```sh
docker start -i -a irpf
```

Para remover tudo:
```sh
docker-compose down --rmi all
```

Para forçar a substituição do container:
```sh
docker-compose up --force-recreate
```
