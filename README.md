# Blood Service Management System

A web-based blood service management system that connects hospitals, blood banks, and delivery partners to facilitate emergency blood requests and donations.

## 🩸 Features

### 🏥 Multi-User Login System
- **Hospital Login**: Register and login for hospitals
- **Blood Bank Access**: Dedicated access for blood banks
- **Delivery Partner Portal**: Interface for delivery partners
- **Emergency Access**: Quick access for urgent situations

### 🔍 Blood Search & Discovery
- Search blood by state, district, and blood group
- Filter available blood units by location
- Real-time blood bank information
- Interactive maps integration

### 🏪 Blood Bank Management
- View available blood banks
- Check blood type availability
- See unit quantities
- Direct ordering system

### 📱 Order Management
- Place blood orders with required units
- Hospital information integration
- WhatsApp request system (planned)
- Order tracking capabilities

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server setup required - runs entirely in browser

### Installation
1. Clone or download the project files
2. Open `login.html` in your web browser
3. Start using the application immediately

### File Structure
```
p-html/
├── login.html          # Main login page
├── dashboard.html      # User dashboard
├── search-blood.html   # Blood search interface
├── blood-banks.html    # Blood bank listings
├── order.html          # Blood ordering system
├── css/
│   └── style.css       # Application styling
└── scripts/
    ├── dashboard.js    # Dashboard functionality
    └── blood-banks.js  # Blood bank data management
```

## 💻 Usage

### For Hospitals
1. **Registration/Login**:
   - Select "Hospital" from dropdown
   - Enter email and password
   - New hospitals are automatically registered
   - Existing hospitals can login with credentials

2. **Search Blood**:
   - Navigate to "Search Blood"
   - Select state, district, and blood group
   - View available options

3. **Place Orders**:
   - Browse blood banks
   - Click "Order" for required blood type
   - Specify units needed
   - Submit WhatsApp request

### For Blood Banks
- Access dedicated blood bank interface
- Manage inventory and availability
- Process incoming requests

### Emergency Access
- Quick access bypass for urgent situations
- Direct dashboard access without login

## 🛠️ Technical Details

### Technologies Used
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Storage**: Browser localStorage for data persistence
- **Maps**: Google Maps integration
- **Communication**: WhatsApp API (planned)

### Data Storage
- Hospital data stored in browser localStorage
- Persistent across browser sessions
- No external database required
- JSON format for data structure

## 📊 Data Management

### Hospital Data Structure
```javascript
{
    hospitalId: 0,
    emailId: "hospital@example.com",
    password: "securepassword"
}
```

### Blood Bank Data Structure
```javascript
{
    name: "City Blood Bank",
    bloodType: "O+",
    units: 5,
    location: "City Center"
}
```

## 🔒 Security Features

- Client-side password validation
- Duplicate email prevention
- Input sanitization
- Secure localStorage implementation

## 🚧 Planned Features

- [ ] WhatsApp integration for order requests
- [ ] Real-time blood bank inventory updates
- [ ] Delivery partner tracking system
- [ ] SMS notifications
- [ ] Advanced search filters
- [ ] Blood donation scheduling
- [ ] Analytics dashboard
- [ ] Mobile app version

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Development Notes

### Adding New Features
- HTML files for new pages
- CSS updates in `css/style.css`
- JavaScript functionality in `scripts/` directory
- localStorage for data persistence

### Testing
- Open `login.html` in browser
- Test registration and login flows
- Verify data persistence across page refreshes
- Check navigation between pages

## 📞 Support

For support and questions:
- Create an issue in the repository
- Check existing documentation
- Review code comments for implementation details

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

**Note**: This is a frontend-only implementation. For production use, consider adding:
- Backend server with database
- User authentication system
- Real-time data synchronization
- Mobile responsiveness improvements
- Security enhancements