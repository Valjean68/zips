sobre flask en serio:

primero, si por alguna erxtraña rqazon estas en D:, pones en el cmd D: y te deja donde queres

segundo, francia

tercero:

- pone python en el cmd y descargalo asi
- pip install flask
- pip install flask_sqlalchemy
- python "app.py"

y q el cielo nos guarde q se cambie este codigo proq se va al chorizo todo, particularmente

app=Flask(__name__)
app.secret_key='qonda'
app.config['SQLALCHEMY_DATABASE_URI']='sqlite:///users.sqlite3'
app.config['SQLALCHEMY_TRACK_MODIFICATIONS']=False


db=SQLAlchemy(app)

app.app_context().push()

db.create_all()
