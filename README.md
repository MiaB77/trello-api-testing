# Trello API Testing Suite

Automated API tests for Trello using Postman and Newman.

## 📋 Project Overview

This project contains a Postman collection that tests the Trello REST API, covering the full board lifecycle: creating boards, lists, cards, moving cards, and deleting boards.

## 🗂️ Collection Structure

| Folder | Requests |
|--------|----------|
| Boards | Create, Get, Delete Board |
| Lists | Create TODO and DONE lists |
| Cards | Create Card, Move Card to DONE |
| Members | Get Boards that Member belongs to |

## ✅ What is tested

- Status codes
- Response body fields
- Board properties (name, closed status, permission level)
- Card movement between lists
- Member board access

## 🛠️ Tools Used

- [Postman](https://www.postman.com/)
- [Trello REST API](https://developer.atlassian.com/cloud/trello/rest/)
- [Newman](https://github.com/postmanlabs/newman)

## 🚀 How to Run

### In Postman
1. Import `Trello API.postman_collection.json`
2. Add your `trelloKey` and `trelloToken` as collection variables
3. Run the collection

### With Newman
```bash
newman run "Trello_API_Collection.json"

## 🔑 Authentication

This project uses Trello API Key and Token. To get yours:
1. Go to https://trello.com/power-ups/admin
2. Generate your API Key and Token

## 👤 Author

MiaB77
