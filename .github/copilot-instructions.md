# Copilot Workspace Instructions

## Development Checklist

Before making or committing changes, verify:

- [ ] `dotnet build SocOps/SocOps.csproj` passes with no errors
- [ ] `dotnet run --project SocOps/SocOps.csproj` starts the dev server
- [ ] Code follows C# naming and style conventions
- [ ] No unused variables or imports remain

## Project Overview

**Soc Ops** is a Blazor WebAssembly app for Social Bingo built on .NET 10. The app is a workshop lab that teaches frontend and agent-driven development with GitHub Copilot.

## Architecture

```
SocOps/
├── Components/     # Reusable Blazor UI components
│   ├── BingoBoard.razor
│   ├── BingoSquare.razor
│   ├── BingoModal.razor
│   ├── GameScreen.razor
│   └── StartScreen.razor
├── Data/           # Static question data
│   └── Questions.cs
├── Models/         # Domain models and game state
├── Pages/          # Routable pages
│   └── Home.razor
├── Services/       # Game logic and state management
│   ├── BingoGameService.cs
│   └── BingoLogicService.cs
└── wwwroot/        # Static assets and CSS
    └── css/app.css
```

## Key Commands

```bash
cd SocOps
dotnet run
# or from repo root:
# dotnet run --project SocOps/SocOps.csproj

dotnet build SocOps/SocOps.csproj
```

> Note: This workspace does not currently include a test project, so `dotnet test` is not available by default.

## Styling Notes

- Uses custom utility classes defined in `SocOps/wwwroot/css/app.css`
- Prefer composable styles like `.flex`, `.grid`, `.items-center`, `.p-4`, `.bg-accent`, and `.text-gray-700`
- Keep component styling simple and consistent with the existing Blazor layout

## Useful References

- Root README: `README.md`
- Workshop guide: `workshop/GUIDE.md`
- Project checkpoints overview: `.solutions/README.md`
- CSS utility guidance: `.github/instructions/css-utilities.instructions.md`
- Frontend design guidance: `.github/instructions/frontend-design.instructions.md`
