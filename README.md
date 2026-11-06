# Social DM Inbox Automation

An AI-powered automation system that receives customer messages from social media, classifies them into categories, and stores them in Airtable for easy management.

## Project Overview

This project automates the process of handling social media direct messages (DMs) using Make.com, OpenAI, and Airtable.

When a customer sends a message, the system analyzes it using AI, identifies its category, generates a short explanation, and saves the information in Airtable.

## Technologies Used

- **Make.com:** Workflow automation
- **OpenAI:** AI-based message classification
- **Airtable:** Data storage and management
- **Hoppscotch:** Webhook testing

## Workflow

1. Receive customer messages through a custom webhook.
2. Parse incoming JSON data.
3. Analyze the message using OpenAI.
4. Classify the message and generate a reason.
5. Parse the AI-generated JSON response.
6. Store the customer message and classification in Airtable.

## Message Categories

- Product Inquiry
- Order Status
- Return/Refund
- Availability
- Other

## Airtable Fields

- Sender
- Platform
- Message
- Category
- Reason

## Testing

The automation was tested with different customer messages to verify all five categories. Test records were successfully stored in Airtable.

## Error Handling

A Retry error handler is configured for the Airtable record-creation module, with incomplete execution storage enabled in Make.com.

## Project Files

- `Social-DM-Inbox-Blueprint.json` – Make.com workflow blueprint.

## Future Improvements

- Connect real social media platforms.
- Add automatic customer replies.
- Support image-based customer inquiries.
- Add notifications for important messages.

## Author

Developed as part of the Think AI Works internship project.


## Project Demo

Watch the complete project demonstration:

[Social DM Inbox Automation – Loom Demo](https://www.loom.com/share/d2093396909248e987ebf5316612dc55)

