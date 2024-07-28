# An Automatic Email Reply System for Film Equipment Rental Service
## Objective:
Design and implement alangchain based system that classifies incoming emails into three
categories and executes specific actions based on the category. The system should enhance
customer interaction by providing automated responses tailored to inquiries, reviews, and
assistance requests.
## Categories and Actions:
### 1. Inquiry Handling:
- Database: Develop an SQL database to store details about film equipment.
- Action: When an inquiry email is received, check the database for item
availability.
  - If available, reply with the item's price.
  - If not available, suggest similar available items.
### 2. Review Handling:
- Positive Reviews: Thank the sender and encourage them to share their
experience on social media.
- Negative Reviews: Escalate to the CRM system for follow-up with a phone call
from customer service and offer a gift voucher in the reply.
### 3. Assistance Request Handling:
- Documentation: Create a document with frequently asked questions about film
equipment using ChatGPT or from equipment manuals.
- RAG Pipeline: Use a Retrieval-Augmented Generation approach to search for
solutions to reported equipment issues. (As of now, Not working completely.)
  - If a suitable solution is found, provide it in the reply.
  - If no solution is found, escalate the issue to customer service.
### 4. General Handling:
- Forwarding: Emails that do not fit into the above categories should be forwarded
to customer service for further evaluation.

## Database Schema
As of now only one relation is considered as we are dealing only with the category, quantity, rental price details of an equipment.
![DatabaseSchema](https://github.com/user-attachments/assets/8f9c4af4-ca6d-4b64-81af-a5fd81f3abee)

## Flowchart of entire procedure



