# Learn Git Branch - Comandos
Comandos usados nos exercícios do Learn Git Branch.

## Sequência introdutória

### 1. Introdução aos commits no Git
```bash
git commit
```

```bash
git commit
```

### 2. Branches no Git

```bash
git checkout -b bugFix
```

### 3. Merge no Git

```bash
git checkout -b bugFix
```

```bash
git commit
```

```bash
git checkout main
```

```bash
git commit
```

```bash
git merge bugFix
```

### 4. Introdução ao rebase

```bash
git checkout -b bugFix
```

```bash
git commit
```

```bash
git checkout main
```

```bash
git commit
```

```bash
git checkout bugFix
```

```bash
git rebase main
```

## Acelerando

### 1. Solte a sua cabeça

```bash
git checkout C4
```

### 2. Referências relativas (^)

```bash
git checkout bugFix^
```

### 3. Referências relativas #2 (~)

```bash
git checkout HEAD^
```

```bash
git branch -f main C6
```

```bash
git branch -f bugFix HEAD^
```

### 3. Revertendo mudanças no Git

```bash
git reset HEAD^
```

```bash
git checkout pushed
```

```bash
git revert HEAD
```

## Movendo trabalho por aí

### 1. Introdução ao cherry-pick

```bash
git cherry-pick C3 C4 C7
```

### 2. Introdução ao rebase interativo

```bash
git rebase -i HEAD~4
```

## Sortidos

### 1. Pegando um único commit

```bash
git rebase -i HEAD~3
```

```bash
git rebase bugFix main
```

### 2. Malabarismo com commits

```bash
git rebase -i HEAD~2
```

```bash
git commit --amend
```

```bash
git rebase -i HEAD~2
```

```bash
git rebase caption main
```

### 3. Malabarismo com commits #2

```bash
git checkout main
```

```bash
git cherry-pick C2
```

```bash
git commit --amend
```

```bash
git cherry-pick C3
```

### 4. Tags no Git

```bash
git tag v1 side^
```

```bash
git tag v0 main~2
```

```bash
git checkout v1
```

### 5. Git Describe

```bash
git checkout v1
```

## Temas avançados

### 1. Fazendo mais de 9000 rebases

```bash
git rebase main bugFix
```

```bash
git rebase bugFix side
```

```bash
git rebase side another
```

```bash
git rebase another main
```

### 2. Múltiplos pais

```bash
git branch bugWork main^^2^
```

### 3. Espaguete de branches

```bash
git checkout one
```

```bash
git cherry-pick C4 C3 C2
```

```bash
git checkout two
```

```bash
git cherry-pick C5 C4 C3 C2
```

```bash
git branch -f three C2
```