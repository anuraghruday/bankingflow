# BankingFlow-AWS-Lambda

**BankingFlow** is an AI-driven chatbot built to simplify banking operations. It assists customers by checking account balances and transferring funds seamlessly, all powered by AWS serverless technology.

## Tools & Technologies
- **Amazon Lex**: Enables natural language interactions.
- **AWS Lambda**: Handles backend processing without server management.
- **Python**: Implements the core business logic.
- **AWS CloudFormation**: Automates infrastructure deployment.

## Key Features

- **Intents & Slot Types**
  - Developed specific intents such as `WelcomeIntent`, `CheckBalance`, and `TransferFunds` to address common banking queries.
  - Configured various slot types to capture user details effectively, ensuring smooth and natural interactions.

- **Custom Slots & Security Enhancements**
  - Created custom slots for different account types (Checking, Savings, Credit) to tailor the conversation to user needs.
  - Integrated validation prompts for date of birth verification, adding an extra layer of security.

- **Balance Inquiry with Context Awareness**
  - The `CheckBalance` intent retrieves account balances based on user inputs while using context carryover to avoid repetitive prompts.

- **Efficient Funds Transfer**
  - The `TransferFunds` intent facilitates fund transfers by collecting multiple pieces of information such as `sourceAccountType`, `targetAccountType`, and `transferAmount` in a single interaction.

- **Dynamic Backend Integration**
  - Integrated with AWS Lambda to process requests and deliver real-time responses, making the bot capable of handling complex transactions like balance inquiries and fund transfers.

- **Automated Deployment**
  - Utilizes AWS CloudFormation to deploy and manage the entire chatbot infrastructure automatically, ensuring a consistent and reliable setup.

- **Enhanced User Experience**
  - Implements confirmation prompts and context carryover to minimize redundant information requests, thereby improving overall interaction efficiency.

BankingBot leverages modern cloud services to deliver a secure, efficient, and user-friendly banking experience.
