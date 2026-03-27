#  Engineering Summer Internship Project: Development of Intelligent Search Engine

## Table of Contents
1. [Project Overview](#project-overview)
2. [Development Environment](#development-environment)
3. [Data Collection and Preparation](#data-collection-and-preparation)
4. [Application Development](#application-development)
5. [Technologies Used](#technologies-used)
6. [Conclusion](#conclusion)

--- 

### Project Overview
Development of an intelligent search engine about illnesses, designed to simplify the searching process and help users find accurate information efficiently. The search engine provides auto-suggestions, spelling corrections, and displays search results with relevant contextual information.

---

### Development Environment

**Hardware Specifications**
- Operating System: Windows 10
- Processor (CPU): 4 physical cores, 8 logical threads
- Memory (RAM): 8 GB at 2667 MHz
- Storage: HDD, 932 GB
- Graphics Card (GPU): Intel(R) Iris(R) Xe Graphics, 128 MB video memory

**Software Specifications**
- VS Code and PyCharm (with Jupyter Notebook support)
- Python 3
- Libraries: Pandas, TensorFlow, re, NLTK, Requests, BeautifulSoup, logging, SpellChecker, Flask

---

### Data Collection and Preparation

**Objectives**
- Create a dataset of textual information about human illnesses
- Tailor the data to project requirements for accurate and relevant results

**Process**
1. **Collecting Data**
   - Extracted textual content from relevant web pages using BeautifulSoup
   - Focused on `<p>` tags to gather paragraph-level text
2. **Preparing Data**
   - Compiled text into a list of dictionaries, one per page
   - Converted into a Pandas DataFrame and saved as a CSV for processing

---

### Application Development

**Search and Result Pages**
- Created with HTML and CSS
- **Search Page (index.html)**
  - Interactive form with search input and dynamic suggestion list
  - Responsive layout and clean styling
- **Results Page (results.html)**
  - Displays search query and contextual search results
  - Shows occurrence count and sentences containing the search term

**JavaScript Features**
- Form submission without page reload
- Fetch search results from Flask backend
- Autocomplete suggestions and corrected query handling

**Python Backend**
- Flask app with routes for `/`, `/search`, `/autocomplete`
- Functions:
  - Fetch data from CSV
  - Index words with sentence positions
  - Remove stop words
  - Apply stemming (PorterStemmer)
  - Correct spelling (SpellChecker)
  - Generate autocomplete suggestions
  - Search function to return relevant results

**CSS Styling**
- Body: Serif fonts, soft blue background, centered layout
- Headings: Large, uppercase, centered
- Search form: Flexbox layout, padded input and buttons, hover effects for submit button

---

### Technologies Used
- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Python, Flask  
- **Data & NLP:** Pandas, NLTK, TensorFlow, SpellChecker  
- **Web Scraping & Utilities:** BeautifulSoup, Requests, logging, re
---

### Conclusion
This project demonstrates the creation of a specialized search engine for illnesses using NLP and web technologies. It required building a custom dataset, developing intelligent search and suggestion functionalities, and designing a user-friendly interface.  
Through this project, I enhanced my skills in **Python, NLP, Flask, HTML, CSS, and JavaScript**, and gained hands-on experience in integrating AI-driven features into a practical web application.


