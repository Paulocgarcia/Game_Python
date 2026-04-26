# Game_Python
 🎮 Jogo Pedra, Papel e Tesoura em Python

Este projeto é uma implementação simples do clássico jogo Pedra, Papel e Tesoura, desenvolvido em Python como parte dos estudos de fundamentos da linguagem.

O objetivo é praticar conceitos essenciais como:

Entrada e saída de dados
Manipulação de strings
Estruturas condicionais (if, elif, else)
Lógica de programação
📚 Contexto do Projeto

Este projeto faz parte do estudo:

Fundamentos de Linguagem Python - Do Básico a Aplicações de IA
Estudo de Caso 2: Construção de um Game

🧠 Lógica do Jogo

O jogo funciona para 2 jogadores, onde cada um escolhe entre:

pedra
papel
tesoura

As regras são:

Pedra vence Tesoura
Tesoura vence Papel
Papel vence Pedra
Jogadas iguais resultam em empate
⚙️ Etapas do Algoritmo
Exibir mensagem inicial
Receber entrada dos jogadores
Normalizar os dados (minúsculas e sem espaços)
Comparar as jogadas
Exibir o resultado
🧾 Pseudo-código
INÍCIO

ESCREVA "--- Jogo Pedra, Papel e Tesoura (2 Jogadores) ---"
ESCREVA "Regras: Escolham entre 'pedra', 'papel' ou 'tesoura'."

LEIA jogada do Jogador 1
LEIA jogada do Jogador 2

CONVERTA jogadas para minúsculas e remova espaços

SE jogadas forem iguais:
    ESCREVA "Empate"
SENÃO SE Jogador 1 vencer:
    ESCREVA "Jogador 1 venceu"
SENÃO:
    ESCREVA "Jogador 2 venceu"

ESCREVA "Fim de jogo"

FIM
💻 Código em Python
jogada_jogador1_inicial = input("Jogador 1: ")
jogada_jogador2_inicial = input("Jogador 2: ")

opcoes_validas = ("pedra", "papel", "tesoura")

jogada_jogador1 = jogada_jogador1_inicial.lower().strip()
jogada_jogador2 = jogada_jogador2_inicial.lower().strip()

print("-" * 25)
print(f"Jogador 1 escolheu: {jogada_jogador1}")
print(f"Jogador 2 escolheu: {jogada_jogador2}")
print("-" * 25)

if jogada_jogador1 not in opcoes_validas or jogada_jogador2 not in opcoes_validas:
    print("Jogada inválida!")

elif jogada_jogador1 == jogada_jogador2:
    print("Empate!")

elif (
    (jogada_jogador1 == "pedra" and jogada_jogador2 == "tesoura") or
    (jogada_jogador1 == "tesoura" and jogada_jogador2 == "papel") or
    (jogada_jogador1 == "papel" and jogada_jogador2 == "pedra")
):
    print("Jogador 1 venceu!")

else:
    print("Jogador 2 venceu!")
    
🚀 Como Executar

https://colab.research.google.com/github/Paulocgarcia/Game_Python/blob/main/Jogo_Pedra_Papel_Tesoura.ipynb


🎯 Aprendizados

Com este projeto, foram praticados:

Estruturas condicionais
Tratamento de entrada do usuário
Boas práticas com strings (lower() e strip())
Organização lógica de algoritmos
 
👨‍💻 Autor

Paulo Cesar Garcia
Estudante de Análise e Desenvolvimento de Sistemas
