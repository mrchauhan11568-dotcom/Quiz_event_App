# 1. Download Zip file 

# 2. Setup Python environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt 

# 3. Setup Frontend (Tailwind)
npm install
npm run build 

# 4. Run Migrations & Create Superuser
python manage.py migrate
python manage.py createsuperuser 

# 5. Run Server
python manage.py runserver