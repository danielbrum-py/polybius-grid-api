# 🔐 Text Encoder API (Grid Cipher)

## 📌 Sobre o projeto

Este projeto tem como objetivo desenvolver uma API capaz de codificar e decodificar textos utilizando um sistema baseado em matriz (grid), onde cada caractere é representado por uma coordenada (linha, coluna).

A aplicação foi criada com foco em praticar conceitos fundamentais de programação e simular a construção de um serviço real, onde dados são processados via requisições HTTP e retornados em formato estruturado.

---

## 🎯 Objetivos do projeto

* Implementar um sistema de codificação de texto baseado em coordenadas
* Desenvolver o processo inverso (decodificação)
* Praticar construção de APIs com Python
* Trabalhar com transformação e mapeamento de dados

---

## 🛠️ Tecnologias utilizadas

* Python
* Pandas
* Flask

---

## 🧹 Etapas do projeto

### Estruturação dos dados

* Criação de um DataFrame personalizado
* Definição de uma matriz de caracteres
* Organização das posições (linha e coluna)

### Lógica de codificação

* Conversão de caracteres em coordenadas
* Tratamento de espaços e caracteres não encontrados
* Estruturação da saída em formato de texto

### Lógica de decodificação

* Leitura de coordenadas
* Conversão de coordenadas em caracteres
* Reconstrução do texto original

### Desenvolvimento da API

* Criação de endpoints com Flask
* Recebimento de dados via requisição POST
* Retorno de respostas em JSON

---

## 🔌 Endpoints

### 📍 Codificar texto

**POST** `/codificar`

Entrada:

```json id="y1b2c3"
{
  "texto": "abc"
}
```

Saída:

```json id="z4x5v6"
{
  "resultado": "1,1 1,2 1,3"
}
```

---

### 📍 Decodificar coordenadas

**POST** `/decodificar`

Entrada:

```json id="a7s8d9"
{
  "coords": "1,1 1,2 1,3"
}
```

Saída:

```json id="f0g1h2"
{
  "resultado": "abc"
}
```

---

## 💡 Principais aprendizados

* Manipulação de dados com DataFrame
* Estruturação de funções em Python
* Criação de APIs REST com Flask
* Processamento de dados via requisições HTTP

---

## 🚀 Possíveis melhorias futuras

* Otimização da busca no DataFrame
* Implementação de tratamento de erros mais robusto
* Suporte a novos conjuntos de caracteres
* Deploy da API em ambiente online

---

## 📌 Autor

Projeto desenvolvido por **Daniel Brum** com foco em aprendizado e evolução na área de programação e dados.
