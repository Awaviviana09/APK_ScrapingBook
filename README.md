<h1 align="center">📚 Book Scraping Application using Google Books API</h1>

<p align="center">
  <b>Interactive Book Data Scraper | Jupyter Notebook | Google Colab</b><br>
  Search, display, and save book information automatically using Python and Google Books API.
</p>

<img width="1919" height="905" alt="image" src="https://i.pinimg.com/736x/23/44/7c/23447cf2d17d6962783578c82c11b3b7.jpg" />

---


| <img width="1919" height="905" alt="image" src="https://github.com/user-attachments/assets/a8eb6ec9-d2cc-424d-a936-2958ad935167" /> | <img width="1919" height="910" alt="image" src="https://github.com/user-attachments/assets/8ea9c460-dff2-4412-8fc6-f73a9064be7b" /> | 
|----|---------------------------------|

---

## 📖 Overview
This project implements an **interactive web scraping application** using the **Google Books API** to help users search, explore, and collect book data based on keywords.  
Users can display book information in a structured HTML layout and save results in **CSV** or **JSON** format.

The program is built using **Python**, **Requests**, **JSON**, and **ipywidgets**, designed for execution in **Jupyter Notebook** or **Google Colab**.

---

## 🧠 Application Workflow

### 🔄 Flowchart
```plaintext
[ Start ]
   ↓
[ Input Keyword ]
   ↓
[ Send HTTP Request to Google Books API ]
   ↓
[ Retrieve & Parse JSON Data ]
   ↓
[ Display Books in HTML Format ]
   ↓
[ (Optional) Save to CSV / JSON ]
   ↓
[ End ]

```

---


## 🧩 Data Structure

```
Each book’s information is stored as a Python dictionary:

book = {
  'judul': 'Judul Buku',
  'penulis': 'Nama Penulis',
  'tanggal': '2022',
  'penerbit': 'Penerbit Buku',
  'deskripsi': 'Deskripsi singkat...',
  'sampul': 'https://link.to/thumbnail.jpg'
}

All books are stored in a list:

books = [book1, book2, book3, ..., book100]

```

---

## 🏗️ Project Structure

```

📦 Book-Scraping-App
 ┣ 📜 scraping_buku.ipynb      # Main notebook file
 ┣ 📜 hasil_scraping.csv       # Saved CSV output
 ┣ 📜 hasil_scraping.json      # Saved JSON output
 ┣ 📁 assets/                  # Screenshots & visuals
 ┣ 📜 README.md                # Documentation file

```

---


## 🧰 Technologies Used

| Category | Tools / Libraries |
|-----------|-------------------|
| **Programming Language** | Python 🐍 |
| **API Source** | Google Books API |
| **Libraries** | Requests, JSON, ipywidgets |
| **Execution Environment** | Jupyter Notebook / Google Colab |
| **Output Formats** | CSV, JSON |

---


## ⚙️ Main Components

| Component | Description |
|------------|-------------|
| **Data Retrieval** | `get_books_data(keyword)` performs 1–3 API requests (pagination) to collect up to 100 book entries. |
| **HTML Display** | `tampilkan_buku_rapi(buku_list)` renders a clean HTML output including cover image, title, author, and short description. |
| **User Interface** | Built using `ipywidgets`, featuring keyword input, search button, save buttons (CSV & JSON), and result display area. |
| **Data Storage** | `simpan_csv()` and `simpan_json()` save book data to external files in their respective formats. |

---


## 🧪 Program Testing

The program was tested using several popular Indonesian keywords:

- 📘 sejarah  
- 📗 dongeng  
- 📙 teknologi  
- 📕 psikologi anak  

✅ All tests successfully retrieved 100 book records (API maximum)  
✅ HTML formatting appeared clean and responsive  
✅ CSV and JSON export functions worked perfectly without errors


---


## 📸 Output Examples

### 🧚‍♀️ Example 1 – Keyword: “Dongeng”
![Dongeng Search Results](https://github.com/user-attachments/assets/c88cf364-410a-45a5-a102-5650b9c8561a)
> The system retrieved 100 books related to **"dongeng"**, displaying title, author, and thumbnail neatly. Data successfully exported to both CSV and JSON files.

---

### 💻 Example 2 – Keyword: “Teknologi”
![Teknologi Search Results](https://github.com/user-attachments/assets/5385856e-1750-42c7-a7db-06cef7bf1ed8)
> The keyword **"teknologi"** returned books focused on innovation, computer science, and AI. The process was fast, accurate, and error-free.

---

### 📚 Example 3 – Keyword: “Psikologi Anak”
![Psikologi Anak Search Results](https://github.com/user-attachments/assets/5a8265eb-b28c-4321-aac4-bb45f2e378ef)
> Displays relevant books in children’s psychology with detailed descriptions. The system rendered HTML layouts effectively even for long text data.

---


## 🧭 How to Run the Program

```

# 1️⃣ Environment Setup
# Use Jupyter Notebook or Google Colab
# Libraries such as requests, json, and ipywidgets are typically preinstalled

# 2️⃣ Run the Notebook
# Open the file scraping_buku.ipynb
# Run all cells (Ctrl + F9 or Run all)

# Interface will appear with:
# - Keyword input box
# - "Cari Buku" button
# - Display area for search results
# - Save buttons for CSV and JSON

# 3️⃣ Perform a Search
# Type a keyword, e.g., filsafat, cerita anak, teknologi, etc.
# Click "Cari Buku" and wait 1–2 seconds for results.

# 4️⃣ Save the Data
# Click "Simpan CSV" to generate hasil_scraping.csv
# Click "Simpan JSON" to generate hasil_scraping.json
# Files are saved automatically in the current directory.

```
---

