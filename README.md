# Weather Forecaster - Ruby on Rails Application

A professional weather forecasting application built with Ruby on Rails that demonstrates geocoding, API integration, caching, and error handling.

## Quick Start

### Prerequisites

- Ubuntu/Debian Linux
- Ruby 3.0.0 or higher
- Node.js (for asset compilation)
- Git

# Update package list
sudo apt update

# Install Ruby and development tools
sudo apt install -y ruby ruby-dev build-essential libssl-dev libreadline-dev zlib1g-dev

# Install RVM
curl -sSL https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm

# Install Ruby 3.0.0
rvm install 3.0.0
rvm use 3.0.0 --default

# Install Bundler
gem install bundler
```

### Setup Application

```bash
# Clone the repository
git clone <repository-url>
cd weather-forecaster

# Install dependencies
bundle install

# Start the server
bin/rails server
```

### Access Application

Open your browser and navigate to: `http://localhost:3000`

### Test the Application

1. Enter any address in the input field
2. Click "Get Weather Forecast"
3. The application will display weather information with coordinates

##unit tests 
bin/rails test

# Run specific test files
bin/rails test test/services/geocode_service_test.rb
bin/rails test test/services/weather_service_test.rb
bin/rails test test/controllers/forecasts_controller_test.rb
bin/rails test test/system/forecasts_test.rb

# Run with verbose output
bin/rails test --verbose

# Run tests in parallel
bin/rails test --parallel
