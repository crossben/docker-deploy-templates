# Use official Ruby image with build tools
FROM ruby:3.2

# Install dependencies
RUN apt-get update -qq && apt-get install -y \
    build-essential \
    libpq-dev \
    nodejs \
    yarn \
    && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /app

# Copy Gemfiles first
COPY Gemfile Gemfile.lock ./

# Install gems
RUN bundle install

# Copy app files
COPY . .

# Precompile assets (optional)
# RUN bundle exec rake assets:precompile

# Expose port Rails dev server listens on
EXPOSE 3000

# Start the Rails server
CMD ["rails", "server", "-b", "0.0.0.0"]
