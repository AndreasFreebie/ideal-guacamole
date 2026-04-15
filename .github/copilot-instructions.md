# Copilot Workspace Instructions

## Mandatory Development Checklist

- [ ] Run linting or analyzer checks
- [ ] `dotnet build SocOps/SocOps.csproj`
- [ ] `dotnet test` when tests exist

## Project Summary

**Soc Ops** is a Blazor WebAssembly Social Bingo workshop app on .NET 10.

## Structure

- `SocOps/Components` — reusable Blazor UI components
- `SocOps/Services` — game state and logic
- `SocOps/Models` — domain models
- `SocOps/Data` — question data
- `SocOps/Pages/Home.razor` — entry page
- `SocOps/wwwroot/css/app.css` — utility-first styles

## Quick Commands

```bash
cd SocOps
dotnet run
# or from repo root:
dotnet run --project SocOps/SocOps.csproj

dotnet build SocOps/SocOps.csproj
```

## Notes

- Styling uses custom utility classes in `SocOps/wwwroot/css/app.css`
- Keep component styling simple and consistent with existing layout

## References

- `README.md`
- `workshop/GUIDE.md`
- `.solutions/README.md`
- `.github/instructions/css-utilities.instructions.md`
- `.github/instructions/frontend-design.instructions.md`
