# 🎧 Análise de Hábitos de Streaming de Música (2026)

Análise exploratória de dados sobre hábitos de consumo de música em plataformas de streaming, com **4.000 registros de ouvintes** ao redor do mundo.

## 📁 Estrutura do projeto

```
analise-streaming/
├── music_streaming_habits_2026.csv   # Dataset original
├── music_streaming_insights.ipynb    # Notebook com a análise completa
└── README.md                         # Este arquivo
```

## 📊 Sobre o dataset

O arquivo `music_streaming_habits_2026.csv` contém **4.000 linhas** e **15 colunas**, sem valores nulos:

| Coluna | Descrição |
|---|---|
| `listener_id` | Identificador único do ouvinte |
| `age` | Idade |
| `country` | País |
| `platform` | Plataforma de streaming (Spotify, Apple Music, etc.) |
| `subscription` | Tipo de assinatura (Free, Premium, Family, Student) |
| `top_genre` | Gênero musical favorito |
| `top_artist` | Artista mais ouvido |
| `daily_listening_minutes` | Minutos de escuta por dia |
| `songs_per_day` | Número de músicas ouvidas por dia |
| `playlists_count` | Número de playlists criadas |
| `skip_rate_pct` | Percentual de faixas puladas |
| `discover_weekly_user` | Se usa playlists de descoberta algorítmica |
| `top_mood` | Humor/contexto predominante de escuta |
| `uses_offline_mode` | Se usa modo offline |
| `podcasts_too` | Se também consome podcasts |

## 🚀 Como rodar

1. Instale as dependências:
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```
2. Abra a pasta no VSCode com as extensões **Python** e **Jupyter** instaladas.
3. Abra `music_streaming_insights.ipynb` e selecione o kernel Python.
4. Rode as células com `Shift+Enter`.

## 🔎 Principais insights

1. **Spotify é líder absoluto**, com ~40% dos ouvintes e liderança em todos os 10 países analisados.
2. **Plano Free é o mais comum** (45,5%), mas a taxa de conversão para Premium é parecida entre plataformas (~30%).
3. **Pop é o gênero mais popular**, mas os "moods" de escuta são bem distribuídos, sem um contexto dominante.
4. A maior parte dos ouvintes está entre **25-34 anos**, e o consumo de podcasts é levemente mais alto entre os mais jovens.
5. Em média, os usuários ouvem **~145 min/dia de música** e pulam ~28% das faixas, com pouca variação por gênero ou plataforma.
6. **Não há correlações fortes** entre idade, tempo de escuta, número de playlists e taxa de skip.
7. A maioria dos usuários usa **recursos de descoberta musical**, sinal maior de engajamento do que o uso do modo offline.

## 🛠️ Tecnologias utilizadas

- Python 3
- pandas
- matplotlib
- seaborn
- Jupyter Notebook (via VSCode)

## 💡 Próximos passos

- Cruzar os dados com métricas de retenção/churn, se disponíveis, para entender se algum desses comportamentos prediz cancelamento de assinatura.
- Segmentar por combinações de variáveis (ex: país + faixa etária) para identificar micro-padrões.