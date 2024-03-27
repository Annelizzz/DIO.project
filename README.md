# DIO.project
Modelo de previsao.AI
import requests

# Dados de exemplo para previsão
data = {'features': [1, 2, 3, 4]}

# Faça uma solicitação POST para o endpoint de previsão
response = requests.post('http://localhost:5000/predict', json=data)

# Obtenha a previsão da resposta JSON
prediction = response.json()['prediction']
print('Previsão:', prediction)
