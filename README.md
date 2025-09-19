# FB (Sandbox)

**Internal documentation. Intended for team members only**

## Project Details

**Name:** TBD

**Internal Codename:** FB

**Internal Namespace:** org.typecrafters.fb

**Engine:** Unity version 6000.0.58f1 LTS

**Platform targets:** PC

**Repository:** Git + LFS

**Production branch:** `main`[[1]](#1)

**Development branch:** `dev`

## Getting Started

1. Download and install [Unity Hub](https://unity.com/download)

2. In Unity Hub, install Unity Editor version 6000.0.58f1 LTS

3. Download and install [Git](https://git-scm.com/downloads)

4. Use a code editor or IDE of your choice. Popular options include: 

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs)

- [JetBrains Rider](https://www.jetbrains.com/rider)

- [Visual Studio Code](https://code.visualstudio.com)

## Workflow

### Cloning the project

```shell
git clone https://github.com/type-crafters/fb-sandbox.git && cd fb-sandbox
```

### Repository conventions

**Feature branches:** `feat/<short-name>`

**Bug fix branches:** `fix/<short-name>`

**Conventional commits:** [See Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0)

```plaintext
<type>(<optional scope>): <description>
empty line
<optional body>
empty line
<optional footer>
```

**Hint: Conventional Commit / SemVer mapping**

| Conventional Commits | Details | SemVer |
| --- | --- | --- |
| `fix` | Patches to bugs in a codebase | `PATCH` (0.0.X) |
| `feat` | Introduction of features to a codebase | `MINOR` (0.X.0) |
| `BREAKING CHANGE` | Introduction of a breaking API change to the codebase. Can be of any type. | `MAJOR` (X.0.0) |

**Pull Requests:**

- Work in a feature/bugfix branch.

- Push branch, open PR into develop.

- Request at least 1 review.

- Resolve conflicts before merge.


## Source Code Convention

| Item | Convention | Example | 
| --- | --- | --- |
| C# Files | PascalCase | `GameManager.cs` |
| Class/Enum/Struct | PascalCase | `class GameManager {}` |
| Interface | PascalCase (prepend with 'I') | `interface IEquippable {}` |
| Method | PascalCase | `void DoSomething() {}` |
| Property | PascalCase | `int Count { get; set; }` |
| Public Field | camelCase | `public string publicGreeting;` |
| Private Field | camelCase (prepend with '_') | `private boolean _isGrounded;` | 

## Notes

#### [1]
This is a sandbox repository, meaning there is no real 'production' branch. The use of `main` as a 'production branch' is intended for completed features that are ready for integration into the project's main repository.