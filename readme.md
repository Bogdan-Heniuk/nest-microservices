
# Nest js microservices

There are 3 services avaliable: gateway, fibonacci, factorial



## Run Locally

Clone the project

```bash
  git clone https://github.com/Bohdan-Heniuk/nest-microservices.git
```

Go to the project directory

```bash
  cd nest-microservices
```

Clone here other microservices

```bash
  git clone https://github.com/Bohdan-Heniuk/fibonacci
```

```bash
  git clone https://github.com/Bohdan-Heniuk/gateway
```

```bash
  git clone https://github.com/Bohdan-Heniuk/factorial
```

Run development docker-compose (rabbitMQ & nginx)

```bash
  docker-compose -f docker-compose-dev.yml up --build
```

Go to projects directories and bootstrap

```bash
  cd gateway
  npm i
  npm run start:dev
```

```bash
  cd fibonacci
  npm i
  npm run start:dev
```

```bash
  cd factorial
  npm i
  npm run start:dev
```

Afteward go http://localhost:3050/swagger to see endpoints avaliable


## Run with k8s


```bash
  kubectl apply -f deployments
```


