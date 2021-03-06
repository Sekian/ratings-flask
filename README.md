# ratings-flask-rest-api

### replicate environtment
virtualenv flask

flask/bin/pip install flask

flask/bin/pip install scikit-learn

### glove file 
glove.42B.300d.txt needs to be at "../data/glove.42B.300d.txt" relative to the python file "./app.py"

### start rest-api
./app.py

### folders structure
    ./data
        glove.42B.300d.txt
        
    ./ratings-flask
        ./flask
            ./bin
            ./lib
            pyvenv.cfg
        app.py
        mlp.joblib
        README.md
    
### api command with curl
curl -i -H "Content-Type: application/json" -X POST -d '{"text":"best product"}' http://localhost:5000/todo/api/v1.0/tasks

curl -i http://localhost:5000/todo/api/v1.0/tasks?text="best+product"

curl -i http://localhost:5000/todo/api/v1.0/tasks/best+product

curl -i http://localhost:5000/todo/api/v1.0/tasks/worst+product

### guides
https://blog.miguelgrinberg.com/post/designing-a-restful-api-with-python-and-flask

https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world

https://blog.miguelgrinberg.com/post/designing-a-restful-api-using-flask-restful