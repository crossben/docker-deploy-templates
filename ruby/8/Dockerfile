# Use Ruby 3.3 (latest stable) until Ruby 4 or 8 is released
FROM ruby:3.3

# Install dependencies
RUN apt-get update -qq && apt-get install -y \
    build-essential \
    libpq-dev \
    nodejs \
    yarn \
    && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /app

# Copy Gemfiles first for better caching
COPY Gemfile Gemfile.lock ./

# Install gems
RUN bundle install

# Copy application files
COPY . .

# Expose Rails default port
EXPOSE 3000

# Run the Rails server
CMD ["rails", "server", "-b", "0.0.0.0"]
