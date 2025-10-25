# FER2013 - Facial Expression Recognition CNN

## 📋 Descrição do Projeto

Este é um projeto de estudo de **Redes Neurais Convolucionais (CNN)** para o reconhecimento de expressões faciais utilizando o dataset **FER2013** (Facial Expression Recognition 2013).

O projeto tem como objetivo:
- Explorar e compreender o dataset FER2013
- Construir e treinar modelos de CNN para classificação de expressões faciais
- Avaliar o desempenho dos modelos
- Estudar técnicas de visão computacional e deep learning

### Expressões Faciais Classificadas
O modelo é capaz de reconhecer as seguintes 7 categorias de expressões:
1. **Angry** (Raiva)
2. **Disgust** (Nojo)
3. **Fear** (Medo)
4. **Happy** (Felicidade)
5. **Neutral** (Neutro)
6. **Sad** (Tristeza)
7. **Surprise** (Surpresa)

## 🛠️ Tecnologias Utilizadas

- **Python** >= 3.12
- **TensorFlow** - Framework para Deep Learning
- **OpenCV** - Processamento de imagens
- **Scikit-learn** - Machine Learning utilities
- **Pandas** - Análise de dados
- **NumPy** - Computação numérica
- **Matplotlib & Seaborn** - Visualização de dados
- **Jupyter Notebook** - Ambiente interativo de desenvolvimento
- **UV** - Gerenciador de pacotes e ambientes virtuais

## 📦 Pré-requisitos

- Python 3.12 ou superior
- UV (gerenciador de pacotes) - [Instruções de instalação](https://docs.astral.sh/uv/)
- Git (opcional)

## 🚀 Guia de Instalação e Configuração

### 1. Clonar ou acessar o repositório

```bash
cd /caminho/para/fer2013
```

### 2. Criar o Ambiente Virtual com UV

Use o comando abaixo para criar um ambiente virtual gerenciado pelo UV:

```bash
uv venv
```

Este comando irá criar um ambiente virtual no diretório `.venv`.

### 3. Ativar o Ambiente Virtual

No Linux/macOS:
```bash
source .venv/bin/activate
```

No Windows:
```bash
.venv\Scripts\activate
```

Você saberá que o ambiente está ativo quando ver `(.venv)` no início da linha do terminal.

### 4. Instalar Dependências com UV

Com o ambiente virtual ativado, instale todas as dependências do projeto:

```bash
uv sync
```

Este comando irá:
- Ler as dependências do arquivo `pyproject.toml`
- Baixar os pacotes necessários
- Instalar todas as bibliotecas especificadas

## 📥 Configuração do Dataset

### Passo 1: Preparar o Diretório de Dados

O dataset será armazenado no diretório `data`. Se ainda não existir, crie-o:

```bash
mkdir -p data
```

### Passo 2: Baixar o Dataset do Kaggle

1. Acesse o dataset em: https://www.kaggle.com/datasets/msambare/fer2013
2. Clique em "Download"
3. O arquivo `fer2013.zip` será baixado

### Passo 3: Mover o Arquivo ZIP para o Diretório Data

Após o download, mova o arquivo ZIP para o diretório `data`:

```bash
mv ~/Downloads/fer2013.zip data/
```

### Passo 4: Extrair o Arquivo ZIP

Extraia o conteúdo do arquivo ZIP:

```bash
cd data
unzip fer2013.zip
cd ..
```

### Passo 5: Estrutura Final do Dataset

Após a extração, você terá a seguinte estrutura de diretórios:

```
data/
├── fer2013.zip (arquivo original)
├── train/
│   ├── angry/
│   ├── disgust/
│   ├── fear/
│   ├── happy/
│   ├── neutral/
│   ├── sad/
│   └── surprise/
└── test/
    ├── angry/
    ├── disgust/
    ├── fear/
    ├── happy/
    ├── neutral/
    ├── sad/
    └── surprise/
```

Cada pasta contém imagens em escala de cinza (.jpg) das expressões faciais correspondentes.

## 📝 Usando o Projeto

### Iniciar o Jupyter Notebook

Com o ambiente virtual ativado, inicie o Jupyter Notebook:

```bash
jupyter notebook
```

Ou para usar JupyterLab (se preferir a interface mais moderna):

```bash
jupyter lab
```

O Jupyter abrirá no seu navegador padrão. Clique em `main.ipynb` para abrir o notebook principal do projeto.

### Estrutura do Notebook

O arquivo `main.ipynb` contém:
- Carregamento e exploração do dataset
- Pré-processamento de imagens
- Construção da arquitetura CNN
- Treinamento do modelo
- Avaliação e visualização dos resultados

## 💻 Comandos Rápidos

**Reativar o ambiente (em sessões futuras):**
```bash
source .venv/bin/activate
```

**Atualizar dependências:**
```bash
uv sync
```

**Desativar o ambiente virtual:**
```bash
deactivate
```

**Remover o arquivo ZIP após extrair (opcional):**
```bash
rm data/fer2013.zip
```

## 📊 Estrutura do Projeto

```
fer2013/
├── main.ipynb           # Notebook principal com todo o código
├── pyproject.toml       # Dependências do projeto
├── README.md            # Este arquivo
├── uv.lock              # Lock file do UV (dependências fixadas)
└── data/
    ├── train/           # Dados de treinamento (28.821 imagens)
    ├── test/            # Dados de teste (7.066 imagens)
    └── fer2013.zip      # Arquivo original (pode ser removido)
```

## 🎯 Próximos Passos

1. Configurar o ambiente conforme as instruções acima
2. Baixar e extrair o dataset FER2013
3. Abrir `main.ipynb` no Jupyter
4. Executar as células do notebook sequencialmente
5. Explorar diferentes arquiteturas de CNN
6. Experimentar com técnicas de augmentação de dados

## 📚 Recursos Adicionais

- [TensorFlow Documentation](https://www.tensorflow.org/)
- [OpenCV Documentation](https://docs.opencv.org/)
- [Kaggle FER2013 Dataset](https://www.kaggle.com/datasets/msambare/fer2013)
- [Jupyter Documentation](https://jupyter.org/)

## 📝 Notas Importantes

- O treinamento do modelo pode levar algum tempo dependendo da sua máquina
- GPU/CUDA pode acelerar significativamente o treinamento
- Certifique-se de ter espaço em disco suficiente (aproximadamente 1-2 GB para o dataset)
- O dataset contém imagens de faces em escala de cinza de diferentes etnias, idades e contextos

## 🤝 Contribuições

Este é um projeto de estudo pessoal. Contribuições e sugestões são bem-vindas!

## 📄 Licença

Dataset FER2013 foi criado por Pierre-Luc Carrier e Aaron Courville em 2013 e é disponibilizado sob licença acadêmica.

---

**Última atualização:** 25 de outubro de 2025
