# PrintEasy - India's Premier Document Printing Service

PrintEasy is a simple yet powerful web application that connects customers with local Xerox shops for hassle-free document printing. This project offers two portals:

- **Customer Portal:** Upload documents, select print options, and place orders with nearby shops.
- **Shop Owner Portal:** Manage orders, update status, and notify customers with real-time notifications.

---

## Features

- **Portal Selection:** Choose between Customer or Shop Owner portal on entry.
- **Customer Portal:**
  - Browse and select from a list of local Xerox shops.
  - Upload multiple documents via drag & drop or file picker (supports PDF, JPG, PNG, DOC, DOCX).
  - Choose print options (Black & White or Color, single/double sided).
  - Specify number of copies and add special instructions.
  - Automatic cost estimation based on print options and document count.
  - Place orders saved locally in browser storage.
  
- **Shop Owner Portal:**
  - Secure login with shop name and password.
  - View all orders placed to the shop with detailed info.
  - Download uploaded documents directly from the browser.
  - Update order status (Pending → Ready → Completed).
  - Send notifications to customers via:
    - Real email (via EmailJS integration or fallback to mailto links).
    - SMS simulation (console logs).
    - Browser notifications (if permitted).
  - Refresh orders without page reload.

- **UI/UX:**
  - Responsive design for desktops and mobiles.
  - Smooth animations and hover effects.
  - Clear success and error messages.
  - File upload size validation (max 10MB per file).
  - Real-time feedback on file uploads and order status changes.

---

## Technologies Used

- HTML5
- CSS3 (with modern styling including gradients, shadows, and animations)
- Vanilla JavaScript (ES6+)
- LocalStorage for data persistence
- EmailJS (optional) for sending real emails

---

## Setup & Usage

1. **Clone or download** the repository.

2. Open the `index.html` file in any modern web browser (Chrome, Firefox, Edge).

3. **Customer Portal:**
   - Click "Enter Customer Portal".
   - Select a Xerox shop.
   - Fill in your details and upload documents.
   - Choose print options and place your order.

4. **Shop Owner Portal:**
   - Click "Enter Owner Portal".
   - Select your shop and enter the password (preset in the code).
   - View and manage orders.
   - Download customer files and update order statuses.
   - Notifications will be sent automatically on status updates.

---

## Email Notification Setup (Optional)

To enable real email notifications via EmailJS:

1. Sign up at [EmailJS](https://www.emailjs.com/).

2. Create an email service (Gmail, Outlook, etc.).

3. Create an email template named `xerox_order_notification`.

4. Replace the placeholders in the JavaScript code with your EmailJS `serviceID`, `templateID`, and `userID`.

5. Test email sending by marking orders as "Ready" or "Completed".

If EmailJS is not configured, the app falls back to opening the default email client with a pre-filled message.

---

## Limitations

- Data and files are stored in browser localStorage; clearing browser data will remove all orders and files.
- Email and SMS notifications are simulated or require EmailJS setup.
- No backend or database integration — suitable for demo or small-scale use.

---

## Future Enhancements

- Backend API for persistent storage and secure authentication.
- Real SMS integration using services like Twilio.
- Admin dashboard for managing shops and users.
- Payment gateway integration.
- Multi-language support.

---

## License

This project is open source and free to use. No license specified.

---

## Screenshots

*(Add screenshots of the Customer Portal, Shop Owner Portal, and notifications here if desired)*

---

## Contact

For questions or contributions, please contact the project maintainer.

---

Enjoy hassle-free printing with **PrintEasy**!
