# Análise de Dados e Modelagem Preditiva para Preço de Apartamentos em Plataforma

## Visão Geral
Este projeto realiza análise de dados e modelagem preditiva em um dataset de aluguéis temporários em uma plataforma na cidade de New York

## Estrutura do Repositório
```
/
├── indicum_dataset.csv
├── indicum_notebook.ipynb 
├── modelo.pkl
├── README.md
└── requirements.txt
```

## Instalação e Execução
1. Clone este repositório:
   ```bash
   git clone https://github.com/Feliperenanfrr/lighthouse-indicum.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd lighthouse-indicum
   ```
3. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate  # Windows
   pip install -r requirements.txt
   ```
4. Execute a análise exploratória e a modelagem (Jupyter Notebook):
   ```bash
   jupyter notebook
   ```
## Previsão de Preço
Para um apartamento com as seguintes características:
```
{'id': 2595,
 'nome': 'Skylit Midtown Castle',
 'host_id': 2845,
 'host_name': 'Jennifer',
 'bairro_group': 'Manhattan',
 'bairro': 'Midtown',
 'latitude': 40.75362,
 'longitude': -73.98377,
 'room_type': 'Entire home/apt',
 'minimo_noites': 1,
 'numero_de_reviews': 45,
 'ultima_review': '2019-05-21',
 'reviews_por_mes': 0.38,
 'calculado_host_listings_count': 2,
 'disponibilidade_365': 355}
```
O modelo estima um preço de **$201.23**.

## Modelo Treinado
O modelo treinado foi salvo no formato `.pkl` e pode ser carregado da seguinte forma:
```python
import pickle
with open('models/modelo.pkl', 'rb') as file:
    modelo = pickle.load(file)
```

## Vídeo Explicativo
O vídeo explicando o desenvolvimento do projeto pode ser acessado [aqui]([link-do-video](https://drive.google.com/file/d/12MeH2xh0Muozra-rAmyiWAya-XTjTUW9/view?usp=sharing)).

## Contato
Caso tenha dúvidas ou sugestões, entre em contato via felipeferreira3146@gmail.com.

