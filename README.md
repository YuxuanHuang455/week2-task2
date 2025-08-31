# week2-task2
git clone https://github.com/<your-org>/<your-repo>.git
cd <your-repo>

# conda
conda env create -f environment.yml
conda activate microtrust
python -m venv .venv && source .venv/bin/activate   # Windows 用 .venv\Scripts\activate
pip install -r requirements.txt
