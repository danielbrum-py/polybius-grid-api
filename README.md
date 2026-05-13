# 🔐 Text Coder API (Grid Cipher)

---

## 📌 About the Project

This project aims to develop an API capable of encoding and decoding text using a grid-based system, where each character is represented by a coordinate (row, column).

The application was created to practice fundamental programming concepts and simulate the development of a real-world service, where data is processed through HTTP requests and returned in a structured format.

---

## 🎯 Project Objectives

- Implement a coordinate-based text encoding system
- Develop the reverse process (decoding)
- Practice API development with Python
- Work with data transformation and mapping

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas
- Flask

---

## 🧱 Project Stages

### 1. 📥 Data Structuring
- Creation of a custom DataFrame
- Definition of a character matrix
- Organization of row and column positions

### 2. 🔐 Encoding Logic
- Converting characters into coordinates
- Handling spaces and missing characters
- Structuring the encoded output

### 3. 🔓 Decoding Logic
- Reading coordinates
- Converting coordinates back into characters
- Reconstructing the original text

### 4. 🌐 API Development
- Creating endpoints with Flask
- Receiving data through POST requests
- Returning responses in JSON format

---

## 🔌 Endpoints

### 📍 Encode Text

**POST** `/encode`

Input:

```json
{
  "text": "abc"
}
```

Output:

```json
{
  "result": "1,1 1,2 1,3"
}
```

---

### 📍 Decode Coordinates

**POST** `/decode`

Input:

```json
{
  "coords": "1,1 1,2 1,3"
}
```

Output:

```json
{
  "result": "abc"
}
```

---

## 📊 API Workflow

### 🔐 Encoding Process
1. The API receives a text string
2. Each character is searched in the grid
3. The character is converted into coordinates
4. The encoded response is returned

### 🔓 Decoding Process
1. The API receives coordinate pairs
2. Each coordinate is mapped back to a character
3. The original text is reconstructed
4. The decoded response is returned

---

## 💡 Key Learnings

- Data manipulation with Pandas DataFrames
- Structuring Python functions and logic
- Building REST APIs with Flask
- Processing data through HTTP requests
- Implementing text transformation systems

---

## 🚀 Future Improvements

- Optimize coordinate search performance
- Implement more robust error handling
- Support additional character sets and symbols
- Add authentication and rate limiting
- Deploy the API to a cloud environment
- Create interactive API documentation

---

## 📌 Author

Project developed by **Daniel Brum** with a focus on learning, backend development, and data processing using Python.
