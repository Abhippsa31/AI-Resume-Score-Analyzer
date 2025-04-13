# 🤖 AI Resume Score Analyzer 

This AI-powered Resume Analyzer uses Natural Language Processing (NLP) to parse resumes, extract skills, score resumes, and recommend personalized learning resources like YouTube courses. Built with Streamlit for an interactive web interface.

---

## 🚀 Features

- 📄 Upload and analyze PDF resumes
- 🧠 Extract skills using NLP (`pyresparser`)
- 📊 Score resumes and provide improvement tips
- 🎯 Recommend skill-based YouTube video courses
- 📁 Admin and User views
- 🔗 Integrated with MySQL to save user data

---

## 🧰 Tech Stack

- Python 🐍
- Streamlit 🌐
- pyresparser (NLP) 🧠
- spaCy, NLTK, pandas, NumPy
- MySQL (via pymysql)
- YouTube video embedding

---

## 📂 Project Structure
📁 AI resume analyzer nlp/ ├── app.py # Main Streamlit frontend ├── Courses.py # Skill-based YouTube course recommendations ├── requirements.txt # Python dependencies ├── Uploaded_Resumes/ # Folder to store uploaded resumes ├── logo/ # Logo used in the app └── .venv/ # Local Python virtual environment (optional)

---

## ⚙️ Installation

```bash
# Clone the repository
git clone https://github.com/your-username/ai-resume-analyzer.git
cd ai-resume-analyzer

# Install dependencies
pip install -r requirements.txt
💻 Running the App
streamlit run app.py
🗃️ Database Schema
CREATE DATABASE cv;

USE cv;

CREATE TABLE user_data (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    email VARCHAR(255),
    skills TEXT,
    resume_score INT
);
🌐 Deployment
You can deploy this app using:

Streamlit Cloud

Render / Heroku (with MySQL add-on)

Make sure to:

Add MySQL credentials securely

Adjust file paths and DB connections if needed

📌 To-Do / Improvements
 Add user authentication

 Use advanced LLMs for better skill extraction

 Add support for DOCX resumes

 Improve scoring algorithm with AI feedback

🙌 Acknowledgements
pyresparser

YouTube Data Source

Streamlit Community

📬 Contact
For questions or collaborations, feel free to reach out at rimun390@gmail.com.

📝 License

---

### 📄 LICENSE (MIT)

```text
MIT License

Copyright (c) 2025 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights  
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell     
copies of the Software, and to permit persons to whom the Software is         
furnished to do so, subject to the following conditions:                       

The above copyright notice and this permission notice shall be included in    
all copies or substantial portions of the Software.                           

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR    
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,      
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE   
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER        
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN     
THE SOFTWARE.
