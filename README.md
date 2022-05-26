
# ETL na prática usando PySpark

Este projeto é um breve treinamento prático sobre a usabilidade de spark com PySpark para processamento de dados. Sua execução será realizada dentro do Google Colab.

## Requisitos para rodar o código

Para rodar o código, será necessário efetuar o download dos arquivos [backtest_results.csv](datasets/backtest_results.csv) e [variables_filtered.csv](datasets/variables_filtered.csv) localizados em [datasets](datasets). Ao longo do código, será requisitado o upload destes dois arquivos.
    
## Configurando variáveis do ambiente no Google Colab

Instale o java dentro da Virtual Machine

```python
!apt-get install openjdk-8-jdk-headless -qq > /dev/null
```

Escolha a versão mais recente do [spark](https://spark.apache.org/downloads.html) para download

```python
!wget -q https://downloads.apache.org/spark/spark-3.1.2/spark-3.1.2-bin-hadoop2.7.tgz
!tar xf /content/spark-3.1.2-bin-hadoop2.7.tgz
```

Crie as variáveis do ambiente

```python
import os
os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"
os.environ["SPARK_HOME"] =  "/content/spark-3.1.2-bin-hadoop2.7"
```


## Documentação

[PySpark documentation](https://sparkbyexamples.com/pyspark/)

