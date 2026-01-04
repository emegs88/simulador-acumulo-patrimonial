# Simulador Prospere Consórcios

Simulador completo de aumento de patrimônio baseado em cotas de consórcio, desenvolvido em React + TypeScript + Vite.

## 🚀 Instalação e Execução

### Pré-requisitos
- Node.js 18+ instalado
- npm ou yarn

### Passos

1. **Instalar dependências:**
```bash
npm install
```

2. **Executar em modo desenvolvimento:**
```bash
npm run dev
```

3. **Acessar no navegador:**
O aplicativo estará disponível em `http://localhost:5173`

## 📊 Gráficos

O simulador inclui **3 gráficos interativos** usando Recharts:

1. **Caixa Acumulado** (Gráfico de Linha)
   - Mostra a evolução do caixa acumulado ao longo dos meses
   - Linha vermelha (#dc2626)
   - Tooltip formatado em R$

2. **Patrimônio Acumulado** (Gráfico de Linha)
   - Mostra a evolução do patrimônio acumulado
   - Linha vermelha (#dc2626)
   - Tooltip formatado em R$

3. **Crédito Liberado por Mês** (Gráfico de Barras)
   - Mostra o crédito liberado em cada mês
   - Barras vermelhas (#dc2626)
   - Tooltip formatado em R$

### Características dos Gráficos:
- ✅ Responsivos (ResponsiveContainer)
- ✅ Formatação de valores em R$ nos tooltips
- ✅ Formatação inteligente do eixo Y (k, M para valores grandes)
- ✅ Grid e estilos alinhados ao tema
- ✅ Otimização de performance (amostragem para datasets grandes)

## 📋 Funcionalidades

- Parâmetros configuráveis
- Tabela mensal editável
- Validações automáticas
- Modo automático
- Resumo com cards
- Gráficos interativos (Recharts)
- Exportação JSON/CSV
- Salvamento automático (LocalStorage)

## 🔧 Tecnologias

- React 18
- TypeScript
- Vite
- Recharts (gráficos)

---

**Desenvolvido para Prospere Consórcios** 🚀