OVERVIEW:

The Cloud Message Scheduler project is designed to help users easily compose a message, choose when it should be sent, and have it delivered automatically via email—like setting a message on a timer. 

User-Friendly Web Interface
We’ve built a clean and responsive interface where users can type in the recipient’s email, write their message, and pick a date and time to send it. Once submitted, the message instantly appears in a live table for easy tracking.

Secure Firestore Integration
Every message is stored in Firebase Firestore with key details like recipient, content, schedule time, and whether it’s been sent or not—ensuring nothing gets lost.

Smart Email Sending System
A custom Node.js script runs in the background to check if it’s time to send any messages. If so, it sends them using Brevo (Sendinblue) and updates their status.

Real-Time Updates
Sent messages are marked as delivered in Firestore, helping users (and us) keep track of what’s completed.

Automation
The project is integrated with Render so that we don't need to manually run the email dispatch script. Instead, it can be triggered automatically at specific intervals (e.g.,every minute).
