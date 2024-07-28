# 🚀 Products Launcher

## 📦 Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/Nest-Microservices-Application/products-launcher
    cd products-launcher
    ```

2. **Initialize submodules:**

    ```sh
    git submodule update --init --recursive
    ```

3. **Configure environment variables:**

    Copy the `.env.template` to `.env` and update the environment variables as needed.

## 🛠️ Development Setup

To start the development environment, follow these steps:

1. **Build and start Docker containers:**

    ```sh
    docker compose up --build
    ```
> [!NOTE]
> This command will build and start all the microservices as specified in the `docker-compose.yml` file.

## 🚀 Production Setup

To set up the production environment, follow these steps:

1. **Build Docker images:**

    ```sh
    docker compose -f docker-compose.prod.yml build
    ```

2. **Run Docker containers:**

    ```sh
    docker compose -f docker-compose.prod.yml up
    ```

## 📂 Project Structure

The project is structured as follows:

- `client-gateway`: The gateway service for client requests.
- `products-ms`: Microservice for managing products.
- `orders-ms`: Microservice for managing orders.
- `payments-ms`: Microservice for handling payments.
- `auth-ms`: Microservice for authentication.

> [!IMPORTANT]
> Each of these directories is a Git submodule linked to its respective repository.
