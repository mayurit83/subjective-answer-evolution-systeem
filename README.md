Project Structure
subjective-answer-evaluation/
│── dataset/               # Training and test data
│── evaluation_model/      # ML model (SVM + TF-IDF)
│── ocr_module/            # OCR for handwritten answers
│── templates/             # HTML frontend pages
│── static/                # CSS, JS, Images
│── manage.py              # Django entry point
│── requirements.txt       # Dependencies
│── README.md

⚙️ Installation & Setup
1️⃣ Clone the repo
git clone https://github.com/your-username/subjective-answer-evaluation.git
cd subjective-answer-evaluation

2️⃣ Create virtual environment & install dependencies
pip install -r requirements.txt

3️⃣ Run database migrations
python manage.py migrate

4️⃣ Train or load ML model
python evaluation_model/train_model.py

5️⃣ Run the server
python manage.py runserver


Open in browser: http://127.0.0.1:8000/

📊 Workflow

Teacher uploads a model answer.

Student submits their subjective answer (typed or scanned).

System applies OCR (if handwritten) + NLP preprocessing.

TF-IDF & SVM model compare similarity.

Marks & feedback are generated automatically.
