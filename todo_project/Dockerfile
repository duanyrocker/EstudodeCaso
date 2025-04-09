# Usa a imagem oficial com Python 3.12
FROM python:3.12-slim

# Define o diretório de trabalho dentro do container
WORKDIR /app

# Copia o arquivo de dependências
COPY requirements.txt .

# Instala as dependências do projeto
RUN pip install --no-cache-dir -r requirements.txt

# Copia o restante dos arquivos do projeto para o container
COPY . .

# Expõe a porta que a aplicação Flask vai usar
EXPOSE 5000

# Comando para rodar o app (ajuste se o run.py estiver em outro lugar)
CMD ["python", "run.py"]
