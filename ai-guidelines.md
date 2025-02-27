# Diretrizes para Geração de Código - Game Programming Patterns

## 1. Princípios Fundamentais

### 1.1 KISS (Keep It Simple, Stupid)
```csharp
// @principle: KISS
// @rules:
// - Evite abstrações desnecessárias
// - Mantenha funções pequenas e focadas
// - Use nomes claros e descritivos
// - Prefira soluções diretas a complexas
```

### 1.2 SOLID
```csharp
// @principle: Single Responsibility
// @rules:
// - Uma classe deve ter apenas um motivo para mudar
// - Separe comportamentos em componentes distintos
// - Evite classes "god object"

// @principle: Open/Closed
// @rules:
// - Extensível para novos comportamentos
// - Fechado para modificações existentes
// - Use interfaces e herança apropriadamente

// @principle: Liskov Substitution
// @rules:
// - Subclasses devem ser substituíveis
// - Mantenha contratos de interface
// - Evite quebrar comportamentos herdados

// @principle: Interface Segregation
// @rules:
// - Interfaces pequenas e específicas
// - Evite interfaces "catch-all"
// - Clientes não devem depender de métodos que não usam

// @principle: Dependency Inversion
// @rules:
// - Dependa de abstrações
// - Evite acoplamento direto
// - Use injeção de dependência
```

## 2. Padrões de Design

### 2.1 Command Pattern
```csharp
// @pattern: Command
// @implementation:
// - Encapsule ações em objetos
// - Permita desfazer/refazer
// - Suporte filas de comandos
// - Use para input handling
```

### 2.2 Flyweight Pattern
```csharp
// @pattern: Flyweight
// @implementation:
// - Compartilhe dados comuns
// - Separe dados intrínsecos/extrínsecos
// - Use factory para instanciação
// - Otimize uso de memória
```

### 2.3 Observer Pattern
```csharp
// @pattern: Observer
// @implementation:
// - Desacople eventos e handlers
// - Suporte múltiplos observers
// - Permita inscrição/cancelamento dinâmico
// - Evite dependências circulares
```

## 3. Padrões de Sequenciamento

### 3.1 Game Loop
```csharp
// @pattern: GameLoop
// @implementation:
// - Separe update e render
// - Mantenha tempo consistente
// - Handle input no momento correto
// - Otimize para performance
```

### 3.2 Update Method
```csharp
// @pattern: Update
// @implementation:
// - Use deltaTime
// - Atualize em ordem correta
// - Evite updates pesados
// - Considere fixed update
```

## 4. Padrões de Otimização

### 4.1 Object Pool
```csharp
// @pattern: ObjectPool
// @implementation:
// - Pré-aloque objetos
// - Reutilize instâncias
// - Gerencie ciclo de vida
// - Evite alocação dinâmica
```

### 4.2 Data Locality
```csharp
// @pattern: DataLocality
// @implementation:
// - Agrupe dados relacionados
// - Use arrays contíguos
// - Minimize cache misses
// - Otimize acesso à memória
```

## 5. Documentação e Comentários

### 5.1 Formato de Documentação
```csharp
/// @class: NomeClasse
/// @purpose: Propósito principal da classe
/// @dependencies: Lista de dependências
/// @patterns: Padrões implementados
/// 
/// @method: NomeMetodo
/// @params: Descrição dos parâmetros
/// @returns: Descrição do retorno
/// @throws: Exceções possíveis
```

### 5.2 Comentários de Implementação
```csharp
// @region: NOME_REGIAO
// @category: Categoria
// @implementation: Detalhes importantes
// @warnings: Pontos de atenção
// @todo: Melhorias futuras
```

## 6. Regras de Performance

```csharp
// @performance: Memória
// - Use structs para tipos pequenos
// - Implemente IDisposable
// - Gerencie referências cíclicas
// - Monitore alocações

// @performance: CPU
// - Otimize loops críticos
// - Use profiling
// - Cache resultados frequentes
// - Evite boxing/unboxing
```

## 7. Validações e Tratamento de Erros

```csharp
// @validation: Input
// - Valide parâmetros
// - Use Debug.Assert
// - Documente pré-condições
// - Trate casos extremos

// @error: Handling
// - Use try/catch apropriadamente
// - Log erros relevantes
// - Mantenha estado consistente
// - Forneça mensagens úteis
```

## 8. Limites do Cursor.AI

```csharp
// @ai: Limitações
// - Não gerar código complexo sem contexto
// - Dividir em partes gerenciáveis
// - Documentar decisões importantes
// - Manter rastreabilidade

// @ai: Capacidades
// - Implementar padrões básicos
// - Gerar documentação
// - Sugerir otimizações
// - Validar estruturas
``` 