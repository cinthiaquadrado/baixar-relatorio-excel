import requests

# URL do link para download do relatório
url = 'https://exemplo.com/link-do-relatorio'

# Caminho para salvar o arquivo baixado
caminho_destino = 'caminho/onde/salvar/o/arquivo/nome_do_relatorio.xlsx'

# Faz a requisição para baixar o arquivo
response = requests.get(url)

# Verifica se a requisição foi bem-sucedida (código 200)
if response.status_code == 200:
    # Abre o arquivo para escrita em modo binário
    with open(caminho_destino, 'wb') as file:
        # Escreve o conteúdo do arquivo na resposta no arquivo local
        file.write(response.content)
    
    print("Download do relatório concluído com sucesso!")
else:
    print("Não foi possível baixar o relatório.")
