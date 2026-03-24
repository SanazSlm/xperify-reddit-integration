# xperify-reddit-integration
This repository contains the backend service that interacts with Reddit’s API to retrieve publicly available posts and comments. The code demonstrates how we access endpoints, process results, and link users back to original Reddit threads.

# Xperify Reddit API Demo

This repository demonstrates how Xperify accesses Reddit's API to retrieve publicly available discussions and direct users back to the original Reddit threads.

## Purpose

Xperify helps users discover relevant Reddit discussions based on their goals and background, such as exam preparation or career transitions.

The goal of this integration is to:

- retrieve publicly available Reddit posts and comments
- identify discussions that may be relevant to a user's situation
- preserve attribution
- link users back to the original Reddit thread for full context and interaction

This demo is intentionally minimal and is designed to show responsible API usage.

## How Xperify Uses Reddit Data

This demo shows a simple workflow:

1. Search or retrieve publicly available Reddit posts from relevant communities
2. Extract limited metadata such as:
   - title
   - subreddit
   - author
   - permalink
   - score
   - comment count
3. Optionally review top-level comments for relevance
4. Return a lightweight structured result
5. Direct users back to the original Reddit thread

## Compliance Principles

This demo is built around the following principles:

- only publicly available Reddit content is accessed
- attribution is preserved
- users are directed back to Reddit for the full discussion
- the demo does not replicate full threads for end-user consumption
- the demo stores only minimal metadata needed for relevance matching and linking

## Example Use Case

A user says:

> I am preparing for IELTS, currently around band 6, weak in writing, and working full-time.

Xperify can use Reddit API data to find relevant public discussions where Redditors described similar situations, then surface those threads with attribution and direct links back to Reddit.

## Project Structure

- `reddit_demo.py` — simple script to call the Reddit API and print structured results
- `.env.example` — example environment variables
- `requirements.txt` — Python dependencies

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-org/xperify-reddit-api-demo.git
cd xperify-reddit-api-demo
