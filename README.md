# Ecossistema de Big Data na AWS

Nesse repositório estão armazenados os arquivos resultados do processo de análise de dados.

Utilizando AWS EMR e Python nesse reposítório há os arquivos de configuração e execução de análise de dados.

Etapas do Projeto: 
Criar um data lake S3 com a estrutura de pastas:
data (upload de arquivo para o bucket)
output
temp

Criar um cluster pelo MrJob e não pelo console
Infraestrutura como código

Criar chave SSH e efetuar o Download .pem file
Configurar MrJob com ID e chave secreta da AWS

Algoritmo de análise de palavras com instalação de bibliotecas
wordcount-test.py
map-reduce-count : contar

Configurar Mrjob

Executar Algoritmo
python3 wordcount-test.py -r emr s3://{your_s3_bucket_name}/data/SherlockHolmes.txt --output-dir=s3://{your_s3_bucket_name}/output/logs1 --cloud-tmp-dir=s3://{your_s3_bucket_name}/temp/
