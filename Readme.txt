1.pip3 install Flask

2.from flask import Flask
app = Flask(__name__)


@app.route("/")
@app.route("/home")
def home():
    return "<h1>Home Page</h1>"
@app.route("/about")
def about():
    return "<h1>About Page</h1>"

if __name__ == '__main__':
    app.run(debug=True)

3.Set enviornment-     export FLASK_APP={{filename}}.py
4.run server - flask run
5.export FLASK_DEBUG=1(du=ebug mode so no need to stop and restart server)
