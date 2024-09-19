# Site Reliability Engineering Health Checker

## Overview

This project is a **Site Reliability Engineering Health Checker** built to monitor the health of a set of HTTP endpoints. The program reads a YAML configuration file containing a list of endpoints, sends HTTP requests every 15 seconds, and logs the availability percentage for each domain being monitored.

The project was implemented in Python using the `requests` library for HTTP requests and `pyyaml` for YAML file parsing.

## Features

- **YAML Configuration**: Define multiple HTTP endpoints (GET/POST) with optional headers and request bodies.
- **Health Checks**: Monitor the health of each endpoint every 15 seconds.
- **Availability Logging**: Log the cumulative availability percentage of each domain in real time.
- **Timeout Handling**: Marks endpoints as DOWN if the response takes longer than 500 ms or if the response status code is not in the 200–299 range.

## Prerequisites

- **Python 3.x**
- Install the required libraries by running the following command:

   ```bash
   pip install -r requirements.txt
