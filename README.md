# Professional Contact Form

A modern, responsive contact form built with React.js and Node.js, featuring email integration, real-time validation, and professional design.

## 🚀 Features

### Frontend (React)
- ✅ **Modern UI/UX** - Clean, responsive design with smooth animations
- ✅ **Real-time Validation** - Client-side form validation with error messages
- ✅ **Loading States** - Visual feedback during form submission
- ✅ **Toast Notifications** - Success/error messages
- ✅ **Mobile Responsive** - Works perfectly on all devices
- ✅ **Character Counter** - Message length indicator
- ✅ **Accessibility** - Proper labels and keyboard navigation

### Backend (Node.js)
- ✅ **Email Integration** - Nodemailer with Gmail SMTP
- ✅ **Auto-Reply System** - Automatic confirmation emails
- ✅ **Rate Limiting** - Prevents spam (5 emails per 15 minutes)
- ✅ **Input Validation** - Server-side validation and sanitization
- ✅ **Security** - Helmet, CORS, and proper error handling
- ✅ **Professional Email Templates** - HTML-formatted emails
- ✅ **Environment Variables** - Secure configuration

## 🛠️ Tech Stack

**Frontend:**
- React 18
- Axios for API calls
- React Toastify for notifications
- CSS3 with animations

**Backend:**
- Node.js
- Express.js
- Nodemailer
- Express Validator
- Express Rate Limit
- Helmet (Security)
- CORS

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- Gmail account with App Password enabled

### Backend Setup

1. **Clone and install dependencies:**
```bash
cd backend
npm install
```

2. **Environment Configuration:**
Create a `.env` file in the backend directory:
```env
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
RECEIVER_EMAIL=admin@yourcompany.com
PORT=5000
CLIENT_URL=http://localhost:3000
```

3. **Gmail App Password Setup:**
   - Enable 2-factor authentication on your Gmail account
   - Go to Google Account settings → Security → App passwords
   - Generate a new app password for "Mail"
   - Use this password in `EMAIL_PASS` (not your regular password)

4. **Start the server:**
```bash
npm run dev
```

### Frontend Setup

1. **Install dependencies:**
```bash
cd frontend
npm install
```

2. **Start the development server:**
```bash
npm start
```

The app will open at `http://localhost:3000`

## 🎯 Usage

1. **Fill out the contact form** with your details
2. **Submit the form** - you'll see a loading state
3. **Receive confirmation** - toast notification for success/error
4. **Email delivery** - both you and the recipient get emails

## 📧 Email Features

### Main Email (to recipient):
- Professional HTML formatting
- Sender details clearly displayed
- Reply-to set to sender's email
- Timestamp included

### Auto-Reply Email (to sender):
- Confirmation of message receipt
- Professional thank you message
- Copy of their original message
- Branded styling

## 🔒 Security Features

- **Rate limiting** - Prevents spam submissions
- **Input validation** - Both client and server-side
- **CORS protection** - Restricted to allowed origins
- **Helmet middleware** - Security headers
- **Email sanitization** - Prevents injection attacks

## 🎨 Customization

### Styling
- Modify `ContactForm.css` for design changes
- Color scheme uses CSS custom properties
- Responsive breakpoints included

### Email Templates
- Edit HTML templates in `server.js`
- Customize email styling and content
- Add company branding

### Validation Rules
- Adjust validation in both frontend and backend
- Modify character limits and requirements

## 🚀 Deployment

### Backend (Heroku/Railway/DigitalOcean)
```bash
npm run build
npm start
```

### Frontend (Vercel/Netlify)
```bash
npm run build
# Deploy the 'build' folder
```

### Environment Variables for Production
Update your hosting platform with:
- `EMAIL_USER`
- `EMAIL_PASS`
- `RECEIVER_EMAIL`
- `CLIENT_URL` (your frontend URL)

## 📱 Responsive Design

- **Desktop**: Full-width form with hover effects
- **Tablet**: Optimized spacing and font sizes
- **Mobile**: Stack layout with touch-friendly inputs

## 🧪 Testing

### Manual Testing Checklist
- [ ] Form validation works
- [ ] Email sending works
- [ ] Auto-reply works
- [ ] Rate limiting works
- [ ] Responsive design works
- [ ] Error handling works

### Load Testing
The rate limiter handles up to 5 emails per 15 minutes per IP.

## 🔧 Troubleshooting

### Common Issues

**Email not sending:**
- Check Gmail App Password is correct
- Verify 2FA is enabled on Gmail
- Check `.env` file configuration

**CORS errors:**
- Ensure `CLIENT_URL` matches your frontend URL
- Check backend is running on correct port

**Form validation errors:**
- Verify all required fields are filled
- Check character limits

## 📄 License

MIT License - feel free to use for personal and commercial projects.

## 👨‍💻 Author

**Ali Kemal Yavaş**
- GitHub: [@Kemalyavas](https://github.com/Kemalyavas)
- Portfolio: [kemalyavas.github.io/Portfolyo-v2.0](https://kemalyavas.github.io/Portfolyo-v2.0)

---

⭐ **Star this repo if you found it useful!**
