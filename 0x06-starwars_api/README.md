# Star Wars API

## Overview
This project involves interacting with the Star Wars API to retrieve and display data related to Star Wars characters and their associated movies. By working through this task, you will gain experience working with APIs, handling HTTP requests, and parsing JSON data.

## Project Objectives
At the end of this project, you should be able to:
- Make HTTP requests to an API endpoint to retrieve data.
- Parse JSON data from an API response.
- Handle asynchronous requests effectively to manage and display information.

## Requirements
- Use **Node.js** for making API requests.
- Handle asynchronous API calls, making sure that data retrieval is efficient and non-blocking.
- Avoid using any external libraries (no `axios`, `request`, etc.) for HTTP requests; rely on built-in modules like `https`.

## Project Structure

This project consists of one main script file that:
1. Fetches information about a Star Wars character based on their ID.
2. Retrieves and lists all the movies in which the character appears, in the correct order.
3. Manages multiple asynchronous requests, ensuring that data is displayed only when all requests are completed.

### Example Usage

```bash
$ node starwars_characters.js <character_id>

