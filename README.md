# Chess Game Engine / Silnik Gry w Szachy

*(Scroll down for English version)*

---

## Wersja Polska

### O projekcie
Rozbudowana, natywna aplikacja szachowa typu desktop, napisana w **Javie 17**. Posiada w pełni interaktywny interfejs graficzny (GUI) stworzony za pomocą Java Swing, kompletną mechanikę gry, efekty dźwiękowe, pasek oceny pozycji oraz wbudowanego przeciwnika komputerowego (AI).

### Główne funkcje
*   **Pełne zasady gry w szachy:** Poprawna implementacja legalnych ruchów, roszady, bicia w przelocie (en passant), promocji piona, mata oraz pata.
*   **Interfejs Graficzny (GUI):** Przejrzysty interfejs szachownicy zrealizowany w Java Swing.
*   **Gra z komputerem (AI):** Możliwość rywalizacji z wbudowanym sztucznym przeciwnikiem.
*   **Pasek Oceny Pozycji (Evaluation Bar):** Wizualna informacja w czasie rzeczywistym, która strona posiada aktualnie przewagę na planszy.
*   **Podświetlanie Ruchów:** Wyraźne wskazywanie wszystkich legalnych ruchów dla wybranej figury, co pomaga m.in. początkującym graczom.
*   **Efekty Dźwiękowe:** Wbudowane powiadomienia audio dla kluczowych wydarzeń w grze (korzystające z `SoundManager`).

### Technologie
*   **Język:** Java 17
*   **Interfejs:** Java Swing / AWT
*   **Narzędzie budowania i zależności:** Maven
*   **Testowanie:** JUnit 5 & Mockito
*   **Pokrycie kodu (Code Coverage):** JaCoCo Maven Plugin

### Struktura projektu
*   `src/main/java/` - Zawiera główną logikę silnika (figury, generowanie ruchów, zasady planszy), logikę AI oraz niestandardowe komponenty GUI (Swing).
*   `src/test/java/` - Posiada testy jednostkowe.
*   `pieces/` & `squareTexture/` - Zasoby graficzne figur, pól szachownicy oraz podświetleń ruchów.
*   `sounds/` - Zasoby dźwiękowe gry.
*   `pom.xml` - Konfiguracja Mavena dla projektu.

### Uruchomienie projektu

#### Wymagania
Upewnij się, że masz zainstalowane **Java 17** oraz **Maven**.

#### Budowanie i uruchamianie
Sklonuj repozytorium i uruchom projekt korzystając z Mavena:
```bash
# Klonowanie repozytorium
git clone https://github.com/kmaill/ChessGameEngine.git
cd ChessGameEngine

# Kompilacja i uruchomienie
mvn clean install
mvn exec:java -Dexec.mainClass="Main"
```
Alternatywnie, możesz otworzyć ten projekt w swoim ulubionym środowisku IDE (np. IntelliJ IDEA, Eclipse) jako "Existing Maven Project" i po prostu uruchomić klasę `Main.java`.

#### Uruchamianie testów
```bash
mvn test
```

### Licencja
Więcej szczegółów znajdziesz w pliku `LICENSE`.

---

## English Version

### About
A feature-rich, desktop-based Chess application built in **Java 17**. It features a fully interactive Graphical User Interface (GUI) created with Java Swing, complete game mechanics, sound effects, an evaluation bar, and a built-in AI opponent. 

### Features
*   **Fully Functional Chess Rules:** Complete implementation of legal moves, castling (roszada), en passant (bicie w przelocie), pawn promotion, checkmate, and stalemate.
*   **Graphical User Interface (GUI):** A clean, custom board UI built with Java Swing.
*   **Play vs AI:** Compete against a built-in computer opponent natively integrated into the engine.
*   **Position Evaluation Bar:** Real-time visual feedback on which side currently yields an advantage.
*   **Move Highlighting:** Clearly highlights all legal moves for a selected piece to help beginners visualize proper moves.
*   **Immersive Sound Effects:** Built-in audio cues for major game events using `SoundManager`.

### Built With
*   **Language:** Java 17
*   **Interface:** Java Swing / AWT
*   **Build Tool & Dependency Management:** Maven
*   **Testing:** JUnit 5 & Mockito
*   **Code Coverage:** JaCoCo Maven Plugin

### Project Structure
*   `src/main/java/` - Contains the core engine logic (Pieces, Move generation, Board rules), AI, and custom Swing GUI components.
*   `src/test/java/` - Contains the unit test suite.
*   `pieces/` & `squareTexture/` - Image assets for pieces, board tiles, and active piece move highlights.
*   `sounds/` - Game audio resources.
*   `pom.xml` - Maven specific project configuration.

### Running the Project

#### Prerequisites
Make sure you have **Java 17** and **Maven** installed on your machine.

#### Build and Run
Clone the repository and run the project using Maven:
```bash
# Clone the repository
git clone https://github.com/kmaill/ChessGameEngine.git
cd ChessGameEngine

# Compile and Run
mvn clean install
mvn exec:java -Dexec.mainClass="Main"
```
Alternatively, you can open the project in your favorite IDE (IntelliJ IDEA, Eclipse, etc.) as an existing Maven project and simply run the `Main.java` class.

#### Running Tests
To run the automated tests using the standard Maven command line:
```bash
mvn test
```

### License
See the `LICENSE` file for more details.
