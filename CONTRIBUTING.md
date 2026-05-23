# Contribuindo para TitanOS

Primeiramente, obrigado por considerar contribuir para TitanOS! É pessoas como você que tornam TitanOS uma distribuição tão ótima.

## Código de Conduta

Este projeto e todos que participam dele são regidos pelo nosso [Código de Conduta](CODE_OF_CONDUCT.md). Ao participar, você deverá seguir este código.

## Como Contribuir

### Reportando Bugs

Antes de criar um relato de bug, por favor faça uma busca nos issues já existentes, pois você pode descobrir que o bug já foi reportado. Se você não encontrar nada, abra um novo issue usando o template de bug report.

**Dicas ao reportar bugs:**
- Use um título descritivo
- Descreva os passos exatos que reproduzem o problema
- Forneça exemplos específicos para demonstrar os passos
- Descreva o comportamento que você observou e aponte qual é o problema
- Explique qual comportamento você esperava ao invés

### Sugerindo Enhancements

As sugestões de enhancement são rastreadas como issues no GitHub. Ao criar um issue de sugestão, inclua:
- Um título descritivo
- Uma descrição detalhada da funcionalidade sugerida
- Exemplos de como a funcionalidade funcionaria
- Possivelmente screenshots ou mockups

### Pull Requests

Os Pull Requests são a melhor forma de propor mudanças no codebase. Nós encorajamos vivamente!

**Processo para fazer um PR:**

1. Fork o repositório e crie sua branch a partir de `main`
2. Se você adicionou código que deveria ser testado, adicione testes
3. Certifique-se de que a suite de testes passa localmente
4. Escreva uma boa mensagem de commit
5. Faça push da sua branch para o seu fork
6. Abra um Pull Request no repositório principal

**Diretrizes para PRs:**
- Siga os padrões de código do projeto
- Escreva mensagens de commit claras e descritivas
- Atualize a documentação conforme necessário
- Adicione testes para novas funcionalidades
- Referencia issues relevantes em seu PR

## Styleguides

### Mensagens de Commit

- Use o tempo presente ("Add feature" ao invés de "Added feature")
- Use o imperativo ("Move cursor to..." ao invés de "Moves cursor to...")
- Limite a primeira linha a 72 caracteres ou menos
- Referencia issues e pull requests liberalmente após a primeira linha
- Tipos de commits:
  - `feat:` Nova feature
  - `fix:` Bug fix
  - `docs:` Documentação
  - `style:` Formatting, missing semicolons, etc
  - `refactor:` Code reorganization
  - `perf:` Performance improvements
  - `test:` Adding or updating tests

Exemplo:
```
feat: add RGB manager to Titan Control Center

Implements RGB control for popular gaming peripherals including
ASUS, Corsair and Razer devices. Includes automatic device detection
and custom lighting profile support.

Closes #123
```

### Código Python

- Use PEP 8
- 4 espaços para indentação
- Máximo de 100 caracteres por linha
- Use type hints

Exemplo:
```python
def calculate_performance(cpu_usage: float, gpu_usage: float) -> dict:
    """Calculate system performance metrics."""
    return {
        "total": (cpu_usage + gpu_usage) / 2,
        "cpu": cpu_usage,
        "gpu": gpu_usage
    }
```

### Código Bash

- Use 4 espaços para indentação
- Sempre use aspas duplas
- Adicione comentários para blocos complexos

Exemplo:
```bash
#!/bin/bash

# Function to check system requirements
check_requirements() {
    if ! command -v pacman &> /dev/null; then
        echo "Erro: pacman não encontrado"
        return 1
    fi
}
```

### Documentação

- Use Markdown para documentação
- Inclua exemplos quando possível
- Links internos devem ser relativos
- Mantenha a estrutura consistente

## Desenvolvimento Local

### Setup do Ambiente

```bash
# Clone o repositório
git clone https://github.com/akra2017linux-rgb/TitanOS.git
cd TitanOS

# Crie um virtual environment
python3 -m venv venv
source venv/bin/activate

# Instale dependências de desenvolvimento
pip install -r requirements-dev.txt

# Configure git hooks
pre-commit install
```

## Processo de Review

Quando você submeter um PR:

1. Um ou mais mantenedores irão revisar seu código
2. Nós buscamos fornecer feedback construtivo
3. Mudanças podem ser solicitadas antes da merge
4. Uma vez aprovado, seu PR será mergeado na branch `main`
5. Seu código será incluído na próxima release

---

Obrigado por contribuir para TitanOS!