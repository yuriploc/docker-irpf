_forked from [samiraguiar](https://github.com/samiraguiar/docker-irpf)_

# Imagem Docker para o Programa IRPF (Imposto de Renda Pessoa Física)

Imposto de Renda Pessoa Física: [O que é?](http://receita.economia.gov.br/interface/cidadao/irpf)

Para executar em ambiente GNU/Linux com Xorg:

```sh
docker run -ti --rm -e DISPLAY --net=host --pid=host --ipc=host irpf
```

**Importante**: Este projeto é apenas uma prova de conceito e não substitui o programa oficial disponibilizado pela Receita Federal, além de não estar associado de forma alguma a este órgão. O autor não se responsabiliza por quaisquer erros na declaração e possíveis problemas com o Fisco causados pela utilização desta imagem.

Para baixar e utilizar a imagem existente:
```sh
docker-compose pull
```

Para executar:
```sh
docker run -ti --rm -e DISPLAY --net=host --pid=host --ipc=host docker.io/matsya/irpf
```
