# Webapp Template

Webapp template/example:

* Backend REST API implemented in Python / Flask
* Frontend app implemented in Typescript / React

## Build and Deploy

The easiest way to deploy the service is by [Docker](https://docs.docker.com/).

```bash
docker-compose up
```

This should start the service in http://localhost:5000/

### Backend (API Server) Development

The backend server is a modified version of [Flask Tutorial](https://flask.palletsprojects.com/en/1.1.x/tutorial/).

You need Python 3. Using a `venv` or `conda` is also recommended. 

```bash
pip install -r requirements.txt
```

To run tests:
```bash
pytest test
```

To start the server:
```bash
export FLASK_APP=server
flask run
```

The default port for the backend http://127.0.0.1:5000/

### Frontend Development

The `./frontend` directory is created by [create-react-app](https://create-react-app.dev/). 

To build the frontend, you will need:
- nodejs (tested on v13.8.0)
- npm (tested on v6.14.6) or yarn (tested on v1.22.0)

```bash
yarn install
# or `npm install`
```

To run the frontend in the development mode on http://localhost:3000, run:
```bash
npm start
```

To build frontend Typescript into a static minified bundle, run:
```bash
npm run build
```