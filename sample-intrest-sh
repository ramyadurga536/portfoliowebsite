#!/bin/bash

# Function to calculate simple interest
calculate_simple_interest() {
  principal="$1"
  rate="$2"
  time="$3"

  # Calculate simple interest
  interest=$(echo "scale=2; $principal * $rate * $time / 100" | bc)

  # Print the result
  echo "Simple Interest: $interest"
}

# Check if the script is called with the right number of arguments
if [ "$#" -ne 3 ]; then
  echo "Usage: ./simple_interest.sh <principal> <rate> <time>"
  exit 1
fi

# Parse the command line arguments
principal="$1"
rate="$2"
time="$3"

# Call the function to calculate simple interest
calculate_simple_interest "$principal" "$rate" "$time"
