
# Nest js microservices

There are 2 services available: fibonacci & factorial



## Run Locally

Clone the project

```bash
  git clone https://github.com/Bohdan-Heniuk/nest-microservices-core.git
```

Go to the project directory

```bash
  cd nest-microservices-core
```

Clone here other microservices

```bash
  git clone https://github.com/Bohdan-Heniuk/nest-microservices-fibonacci
```

```bash
  git clone https://github.com/Bohdan-Heniuk/nest-microservices-gateway
```

```bash
  git clone https://github.com/Bohdan-Heniuk/nest-microservices-factorial
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


