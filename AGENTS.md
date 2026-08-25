# Soc Ops Agent Guide

## Mandatory Checklist

Before finishing any change:

1. **Lint:** run `git diff --check` (no dedicated linter is configured).
2. **Test:** run `cd socops && ./mvnw test`.
3. **Build:** run `cd socops && ./mvnw clean package` for production or dependency changes.
4. Review the diff and keep it scoped to the request.

## Project Map

- `socops/` is a Java 21 Spring Boot app using the Maven wrapper.
- `BingoRestController` serves `game.html` and `GET /api/bingo/fresh-board`.
- `BoardAssembler` is a static, framework-free utility for board creation, toggling, and victory detection. Preserve its immutable returns.
- `model/` contains immutable records; `data/IcebreakerPrompts.java` contains 24 prompts. The 25-cell board has a selected, untoggleable free cell at index 12.
- `game.html` contains the Thymeleaf view and vanilla JavaScript state machine. Browser `localStorage` owns game persistence; the server is stateless.
- `app.css` provides custom utility classes; there is no frontend framework or build tool. Follow [.github/instructions/css-utilities.instructions.md](.github/instructions/css-utilities.instructions.md).
- Extend `BoardAssemblerTests` with focused JUnit 5 tests when changing domain behavior; use direct calls and no mocks.
- Keep 5x5 row-major indexing and support rows, columns, and both diagonals when changing victory logic.

## Documentation

See [README.md](README.md) for commands, [workshop/GUIDE.md](workshop/GUIDE.md) for the intended workflow, and [CONTRIBUTING.md](CONTRIBUTING.md) for contribution requirements.