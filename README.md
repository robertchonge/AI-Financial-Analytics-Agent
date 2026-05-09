
📊 AI-Financial-Analytics-Agent

A web tool that analyzes CSV, Excel, and PDF financial statements using AI.
Auto-generates:

Income & expense breakdown,

Risk insights,

Actionable business recommendations.



---

📦 Tech Stack

Layer	Technologies

Frontend	Next.js (React), Tailwind CSS, Axios
Backend API	Django REST Framework, Pandas, pdfplumber, OpenAI (LLM API)
LLM Engine	GPT-4o API / Claude API / Local LLaMA (optional)
Containerization	Docker (both frontend & backend)



---

📁 Project Structure

finance-insights/
├── backend/                # Django REST backend
├── frontend/               # React Next.js frontend
└── README.md               # (this file)


---

⚙️ Backend Setup (Django + REST API)

Prerequisites:

Python 3.10+

pip


Setup:

cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\\Scripts\\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

API will run at:

http://localhost:8000/api/upload-financials/

Main API:

POST /api/upload-financials/

Input: CSV / XLSX / PDF file.

Output: Rows, columns, and AI-generated insights.




---

🎨 Frontend Setup (Next.js)

Prerequisites:

Node.js 18+


Setup:

cd frontend
npm install
npm run dev

App available at:

http://localhost:3000/

Features:

Upload bank statements (CSV, Excel, or PDF).

View AI-generated summaries and business advice.

Visualize file columns and row count.



---

🐳 Docker Deployment

Both frontend and backend include Dockerfiles.

Example (Backend):

cd backend
docker build -t finance-backend .
docker run -p 8000:8000 finance-backend

Example (Frontend):

cd frontend
docker build -t finance-frontend .
docker run -p 3000:3000 finance-frontend


---

🚀 Future Improvements

Charts (income/expense graphs).

Historical prompt saving.

Multi-user support.

WhatsApp bot version.

Local deployment for Zimbabwean SMEs.



---

👤 Author

Robert Chonge
📧 robertchonge07@gmail.com
