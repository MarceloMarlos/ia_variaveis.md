# Interação com IA — Variáveis em Dart

## 🧠 Introdução

Neste exercício, utilizei a Inteligência Artificial como ferramenta de apoio no aprendizado sobre variáveis na linguagem Dart. As interações abaixo mostram as perguntas que fiz e as respostas geradas, com o intuito de entender conceitos como boas práticas, valores nulos, modificadores como `late`, `final` e `const`, além de métodos aplicáveis a Strings e números.

---

## 💬 Interações com a IA

### 1. Quais as boas práticas em Dart ao declarar variáveis?

**Resposta da IA:**  
Em Dart, boas práticas incluem:
- Declarar variáveis com tipos explícitos para facilitar a leitura.
- Utilizar `final` para variáveis cujo valor não será alterado.
- Usar nomes descritivos e em camelCase.
- Evitar abreviações e nomes genéricos como `x` ou `temp`, exceto em contextos muito curtos.
- Preferir `const` quando o valor for completamente imutável em tempo de compilação.

---

### 2. O que evitar na hora de declarar variáveis em Dart?

**Resposta da IA:**  
Evite:
- Declarar variáveis que nunca serão utilizadas.
- Atribuir valores nulos sem necessidade.
- Usar o modificador `late` sem entender as consequências.
- Declarar variáveis com escopo global desnecessariamente.
- Nomear variáveis de forma confusa ou repetitiva.

---

### 3. Quais cuidados tomar quando crio variáveis com valor nulo trabalhando com Dart?

**Resposta da IA:**  
Dart possui null safety, ou seja, você deve indicar explicitamente se uma variável pode ser nula usando `?`. Sempre inicialize variáveis ou use `late` se tiver certeza de que o valor será atribuído antes do uso. Tome cuidado com variáveis nulas em expressões — utilize `??` (operador de coalescência nula) e `!` (para afirmar que não é nulo) com responsabilidade.

---

### 4. Gostaria de entender quais os benefícios de utilização do modificador `late` no Dart.

**Resposta da IA:**  
O `late` permite declarar variáveis não nulas que serão inicializadas depois. Útil quando a inicialização depende de outra lógica, mas você garante que ela será feita antes do uso. Evita o uso de `?`, mantendo o tipo não nulo.

---

### 5. Quais as diferenças entre `final` e `const` em Dart?

**Resposta da IA:**  
- `final`: O valor é atribuído uma única vez em tempo de execução.
- `const`: O valor é conhecido e fixo em tempo de compilação.
Use `const` quando o valor não depende de lógica e é fixo, como `const pi = 3.14;`. Use `final` quando o valor é definido em tempo de execução e não muda depois, como `final data = DateTime.now();`.

---

### 6. Me traga um exemplo do uso do método `split()` em Dart.

**Resposta da IA:**  
```dart
void main() {
  String texto = "Dart é incrível";
  List<String> palavras = texto.split(" ");
  print(palavras); // [Dart, é, incrível]
}
