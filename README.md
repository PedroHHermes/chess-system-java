# ♟️ Chess System - Java

Sistema de jogo de xadrez desenvolvido em Java utilizando Programação Orientada a Objetos (POO).

## 📋 Sobre o Projeto

Este é um jogo de xadrez completo executado via terminal/console, desenvolvido como projeto educacional do curso de Java COMPLETO da Udemy. O sistema implementa todas as regras do xadrez, incluindo movimentos especiais e lógica de xeque-mate.

## ✨ Funcionalidades

- ♟️ Jogo de xadrez completo no terminal
- 🎯 Movimentos válidos destacados para cada peça
- 🔄 Movimentos especiais implementados:
  - Roque (Castling)
  - En Passant
  - Promoção de Peão
- ⚠️ Detecção de xeque e xeque-mate
- 📊 Lista de peças capturadas
- 🎨 Interface colorida no terminal
- ✅ Validação completa de movimentos

## 🏗️ Estrutura do Projeto

```
chess-system/
│
├── src/
│   ├── application/
│   │   ├── Program.java          # Classe principal
│   │   └── UI.java                # Interface do usuário
│   │
│   ├── boardgame/
│   │   ├── Board.java             # Tabuleiro genérico
│   │   ├── BoardException.java    # Exceções do tabuleiro
│   │   ├── Piece.java             # Peça genérica (abstrata)
│   │   └── Position.java          # Posição no tabuleiro
│   │
│   └── chess/
│       ├── ChessException.java    # Exceções de xadrez
│       ├── ChessMatch.java        # Lógica da partida
│       ├── ChessPiece.java        # Peça de xadrez
│       ├── ChessPosition.java     # Posição no formato xadrez (a1-h8)
│       ├── Color.java             # Enum de cores
│       └── pieces/
│           ├── Bishop.java        # Bispo
│           ├── King.java          # Rei
│           ├── Knight.java        # Cavalo
│           ├── Pawn.java          # Peão
│           ├── Queen.java         # Rainha
│           └── Rook.java          # Torre
```

## 🚀 Como Executar

### Pré-requisitos

- Java JDK 11 ou superior
- Terminal com suporte a cores ANSI (recomendado: Git Bash no Windows, terminal padrão no Linux/Mac)

### Compilação e Execução

```bash
# Compilar o projeto
javac -d out src/application/*.java src/boardgame/*.java src/chess/*.java src/chess/pieces/*.java

# Executar
java -cp out application.Program
```

## 🎮 Como Jogar

1. O jogo utiliza notação algébrica de xadrez (a1-h8)
2. No seu turno, digite a posição da peça que deseja mover (ex: `e2`)
3. O sistema mostrará os movimentos possíveis destacados em azul
4. Digite a posição de destino (ex: `e4`)
5. Peças capturadas são listadas ao lado do tabuleiro
6. O jogo continua até o xeque-mate

### Notação do Tabuleiro

- Colunas: `a` a `h` (esquerda para direita)
- Linhas: `1` a `8` (baixo para cima, perspectiva das brancas)

### Símbolos das Peças

- ♔/♚ - Rei (K)
- ♕/♛ - Rainha (Q)
- ♖/♜ - Torre (R)
- ♗/♝ - Bispo (B)
- ♘/♞ - Cavalo (N)
- ♙/♟ - Peão (P)

## 🎓 Conceitos de POO Aplicados

- **Encapsulamento**: Atributos privados com getters e setters
- **Herança**: Hierarquia de classes (Piece → ChessPiece → peças específicas)
- **Polimorfismo**: Método abstrato `possibleMoves()` implementado por cada peça
- **Abstração**: Classe abstrata `Piece` como base
- **Enumerações**: Enum `Color` para cores das peças
- **Exceções customizadas**: `ChessException` e `BoardException`
- **Composição**: Board contém Pieces, ChessMatch contém Board
- **Sobrecarga**: Construtores e métodos sobrecarregados
- **Sobrescrita**: Métodos sobrescritos de Object (toString, equals)

## 📚 Aprendizados

Este projeto consolida diversos conceitos fundamentais de Java e POO:

- Estruturas de dados (arrays bidimensionais, listas)
- Tratamento de exceções
- Programação defensiva
- Lógica de negócio complexa
- Design de classes e relacionamentos
- Boas práticas de programação

## 🔗 Referências

Projeto desenvolvido no curso **Java COMPLETO - Programação Orientada a Objetos + Projetos** da Udemy, ministrado pelo Prof. Nélio Alves.

## 📝 Licença

Este projeto é de código aberto e está disponível para fins educacionais.

---

Desenvolvido com ☕ e Java
