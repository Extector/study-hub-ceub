# Gêmeo digital: dissipador térmico para Raspberry Pi

Trabalho da disciplina Fundamentos de Engenharia — CEUB.

**Autor:** Luis Gustavo Campos  
**Ano:** 2026

## Proposta

Modelo de dissipador de alumínio 6063 (40 × 40 × 20 mm), com sete aletas, para avaliar o resfriamento de um pequeno sistema com dois Raspberry Pi 4. São comparados cenários sem ventilação e com ventilação forçada.

## Arquivos

- `relatorio-gemeo-digital-ceub-22650630.pdf`: relatório técnico e resultados.
- `dissipador.FCStd`: geometria 3D editável, abrir no FreeCAD.
- `dissipador_desenho-tecnico.pdf`: desenho técnico cotado.
- `dissipador_visualizacao.e2d`: visualização térmica, abrir no Energy2D.
- `simulacao-raspberry.ipynb`: cálculos e gráficos, abrir no Google Colab.

## Como reproduzir

1. Abrir `dissipador.FCStd` no FreeCAD para conferir a geometria.
2. Abrir `dissipador_visualizacao.e2d` no Energy2D e iniciar a simulação.
3. Enviar `simulacao-raspberry.ipynb` ao [Google Colab](https://colab.research.google.com/) e escolher **Ambiente de execução → Executar tudo**.
4. Comparar os gráficos e os cálculos com o relatório técnico.

## Resultados do notebook

| Indicador | Resultado |
|---|---:|
| Temperatura estimada sem ventilador | 111,63 °C |
| Temperatura estimada com ventilador | 58,44 °C |
| Limite de projeto | 80 °C |
| Dilatação livre | 0,0154 mm |
| Tensão térmica teórica, dilatação impedida | 26,5 MPa |
| Consumo elétrico anual estimado | 113,88 kWh |

Os resultados são estimativas de simulação com hipóteses de potência, temperatura ambiente e coeficientes de convecção. Não foram realizadas medições físicas. O Energy2D e o notebook utilizam condições diferentes e não devem ser tratados como medições equivalentes.
