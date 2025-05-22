# 🌀 Fractol - Fractais em C com MiniLibX

Projeto desenvolvido como parte do currículo da 42 School, cujo objetivo é gerar e explorar fractais matemáticos interativos utilizando a biblioteca gráfica [MiniLibX](https://harm-smits.github.io/42docs/libs/minilibx).

## 📸 Demonstração

// Inserir aqui um GIF ou screenshot do fractal em execução (ex: fractal Julia com zoom interativo)

---

## 🚀 Funcionalidades

- Renderização de fractais em tempo real:
  - Mandelbrot
  - Julia (com entrada personalizada)
  - Burning Ship
- Suporte a zoom com scroll do mouse
- Navegação com teclado (opcional)
- Parâmetros ajustáveis via linha de comando
- Sem vazamentos de memória (verificado com Valgrind ✅)

---

## 🧠 Conceitos Matemáticos

Os fractais são gerados a partir de fórmulas iterativas no plano complexo:

- **Mandelbrot:**  
  Zₙ₊₁ = Zₙ² + C, com Z₀ = 0

- **Julia:**  
  Zₙ₊₁ = Zₙ² + C, com Z₀ sendo o pixel, e C fornecido pelo usuário

- **Burning Ship:**  
  Zₙ₊₁ = (|Re(Zₙ)| + i·|Im(Zₙ)|)² + C

---

## ⚙️ Como compilar

// Este projeto é compatível com Linux e requer a biblioteca MiniLibX.

// 1. Instalar dependências (Debian/Ubuntu):
sudo apt-get install libx11-dev libxext-dev libbsd-dev

// 2. Clonar o repositório:
git clone https://github.com/teu-usuario/fractol.git
cd fractol

// 3. Compilar:
make

---

## 🖥️ Como executar

./fractol <fractal_type>

// Parâmetros válidos:
- `julia` → Conjunto de Julia
- `mandelbrot` → Conjunto de Mandelbrot
- `burning_ship` → Burning Ship

// Exemplo:
./fractol julia

Se escolher `julia`, o programa solicitará os valores reais e imaginários para `c`.

---

## 🖱️ Controles

| Ação            | Comando         |
|-----------------|-----------------|
| Zoom In/Out     | Scroll do mouse |
| Fechar janela   | Tecla `ESC` ou botão X |
| Ajustar iterações (opcional) | Botões adicionais (ex: clique direito) |

---

## 🔎 Validação

Verificado com:
- `valgrind` → Sem vazamentos de memória
- `norminette` → Conforme as regras da 42 (se aplicável)

---

## 👨‍💻 Autor

| Nome     | GitHub             | Escola 42 |
|----------|--------------------|-----------|
| Cassiano | [@teu-usuario](https://github.com/teu-usuario) | 42 Lisboa |

---

## 📄 Licença

Este projeto é parte do currículo pedagógico da 42 School. Uso educacional e pessoal.

