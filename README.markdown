# lagproxy
## Laggy proxy for webserver & web service testing

## Description

Lagproxy is a multithreaded laggy proxy using ruby's WEBrick. It supports arbitrary sized delays and variability.

## Requirements

lagproxy requires ruby. It's been tested with 1.9.2, but the 1.8 series should work without any trouble.

## Usage

	# Set up lagproxy
	./lagproxy --delay=2.0 --variance=0.0

	# Test it's working
	http_proxy=http://localhost:8080/ time wget -O /dev/null http://www.google.com 

