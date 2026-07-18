# Projeto Final
Template do Projeto Final da Disciplina **Bancos de Dados**

## Instruções

- [ ] Atender aos requisitos obrigatórios contidos no documento "Roteiro do Projeto Final de Bancos de Dados" disponibilizado no ambiente do GSA da turma.
- [ ] Implementar Readme.md para atender os itens do relatório (opcional).

---

# Dodge the creeps!

Dodge the creeps! é um jogo de sobrevivencia simples desenvolvida na engine Godot utilizando a linguá própria da engine no qual você deve desviar de varios creeps por o maior tempo possivel para que o usuario ganhe uma pontuação maior

## visão geral

---

Este repositório reúne o projeto desenvolvido para a disciplina de **Análise e Projeto de Sistemas Web**.

O objetivo é aplicar conceitos de **Programação Orientada a Objetos (POO)** e **padrões de projeto GoF**, promovendo um código mais organizado, reutilizável e de fácil manutenção.

---

##  Objetivo

Desenvolver uma aplicação em GDScript aplicando conceitos de:

- Programação Orientada a Objetos (POO)
- Organização de classes e métodos
- Padrões de projeto GoF
- Estruturação de sistemas em console
- Boas práticas de desenvolvimento

---

## Funcionamento

-O jogo funciona de maneira simples, ao abrir o jogo, você tera o botão Start, que lhe permitirar começar o jogo.
-Ao começar, você ira utilizar as setas do lado direito do teclado para poder mover o seu personagem
-Evite ser atigindo pela maior quantidade de tempo possível
-Ao morrer você ira recomeçar do zero

---

## Padrões de Projeto Utilizados (GoF)

### Observer (Comportamental)

Quando o Player colide com um inimigo, ele emite o sinal hit. A cena principal (Main) está escutando esse sinal e reage chamando a função de game_over().

### Composite (Estrutural)

A cena Main é o nó pai. Ela gerencia nós filhos que são objetos individuais (como o Player, HUD, ScoreTimer) e também nós que geram outros objetos (como as instâncias dos inimigos). Todos herdam de Node, compartilhando funções básicas como _process() ou _ready().

### Factory Method / Abstract Factory (Criacional)

o script da cena Main, você exporta uma variável do tipo PackedScene para carregar o arquivo do inimigo (Mob.tscn). Quando o timer zera, o código faz mob_scene.instantiate() para fabricar uma nova cópia do inimigo na memória.

### Prototype (Criacional)

A cena Mob criada na documentação funciona como o protótipo do inimigo. Cada vez que um novo creep entra na tela, a Godot clona aquele protótipo original em vez de redefinir o objeto do zero.

---


## Tecnologias utilizadas

-GDScript
- Programação Orientada a Objetos (POO)
- Padrões de Projeto GoF
- Git
- GitHub

---

## Estrutura do Projeto

O projeto foi organizado em cenas com as funções definidas, facilitando manutenção e escalabilidade.

---

## Como executar

1. Baixe o repositório e os arquivos

2. Execute o arquivo executavel: jogo.exe

3. Aperte o butão Start 

---

##  Aprendizados

Durante o desenvolvimento deste projeto foram praticados conceitos como:

- funções
- cenas
- Organização do código
- Separação de responsabilidades entre as classes ou funções
- criação de cenas
- Menus interativos
- Entrada de sinais
- Aplicação de padrões de projeto GoF

---

## Próximas melhorias

Algumas funcionalidades que poderão ser adicionadas futuramente:

- Persistência de dados como: partida mais longa, pontuação maxima
- Mais variações de inimigos
- Sistema de ranqueamento dos jogadores
- 
---

##  Autor

Projeto desenvolvido por **Gabriel Franco** durante a disciplina de **Análise e Projeto de Sistemas Web**.
