FROM maven:3.9-eclipse-temurin-25

RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash - \
    && apt-get install -y nodejs

RUN apt-get update && apt-get install -y \
    git \
    curl \
    wget \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace

RUN mvn --version && node --version && npm --version
