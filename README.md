# final.automaton
## 🤖🔌🧠🔧🏭

# Simulador de Autômatos Finitos

Um simulador de autômatos finitos que recebe um arquivo representando o diagrama de transições e um arquivo com as entradas de testes, executando o autômato correspondente e armazenando os resultados em um arquivo de saída.

## Como Usar

1. **Clone o Repositório:**

```bash
git clone https://github.com/seu-usuario/automato-simulator.git
cd automato-simulator
```
2. Instale as Dependências:

Não há dependências externas. O projeto utiliza apenas as bibliotecas padrão do Python.

3. Execute a Ferramenta:
```py
python main.py arquivo_do_automato.aut arquivo_de_testes.in arquivo_de_saida.out
```
# Formato dos Arquivos

## Especificação da Máquina de Estados (arquivo_do_automato.aut)
```json
{
  "initial": 0,
  "final" : [4,7],
  "transitions": [
    {"from": 0, "read": "a", "to": 1 },
    {"from": 1, "read": "b", "to": 3 },
    {"from": 2, "read": "a", "to": 3 },
    // ...
  ]
}
```
## Entradas para Teste (arquivo_de_testes.in)
```js
palavra de entrada;resultadoesperado
aababababbbababa;1
aababababbbababa;1
// ...
```
# Resultados
Os resultados da simulação serão armazenados no arquivo arquivo_de_saida.out no formato:
```js
palavra de entrada;resultadoesperado;resultadoobtido;tempo
aababababbbababa;1;1;0.007
// ...
```
# Licença
> Este projeto está sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.

# Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para enviar pull requests ou reportar problemas.

# Equipe
João C. F. M. C.

 Projeto desenvolvido como parte da disciplina Teoria da Computação na Universidade Estadual do Norte do Paraná - UENP