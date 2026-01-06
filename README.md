# Dashboard de Fechamentos de Processos

Dashboard interativo para visualização de dados de fechamentos de processos por responsável.

## 📋 Requisitos

- Navegador web moderno (Chrome, Firefox, Edge, Safari)
- Servidor web local (opcional, mas recomendado)

## 🚀 Como executar

### Opção 1: Abrir diretamente no navegador
1. Abra o arquivo `index.html` no seu navegador
2. O dashboard carregará automaticamente os dados do arquivo `Processos.csv`

### Opção 2: Usar servidor local (recomendado)
Para evitar problemas de CORS ao carregar o CSV, use um servidor local:

**Com Python:**
```bash
python -m http.server 8000
```

**Com Node.js:**
```bash
npx http-server
```

**Com PHP:**
```bash
php -S localhost:8000
```

Depois acesse `http://localhost:8000` no navegador.

## 📊 Funcionalidades

- **Métricas Principais**: Total de fechamentos, abertos, saldo atual e taxa de fechamento
- **Gráfico de Barras**: Total de fechamentos por responsável
- **Gráfico de Linha**: Evolução mensal de fechamentos
- **Gráfico Comparativo**: Abertos vs Fechados acumulados
- **Gráfico de Saldo**: Saldo acumulado por responsável
- **Filtros Interativos**: Filtro por responsável e período
- **Tabela de Resumo**: Dados detalhados por responsável

## 📁 Estrutura

- `dashboard.html`: Arquivo HTML único com todo o código (CSS e JavaScript incorporados)
- `Processos.csv`: Arquivo de dados (deve estar na mesma pasta)

## 🛠️ Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript (Vanilla)
- Chart.js (via CDN)

