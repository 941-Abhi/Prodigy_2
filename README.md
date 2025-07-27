# Employee Management System

A modern, responsive web application for managing employee records with full CRUD (Create, Read, Update, Delete) operations.

## Features

- ✨ **Modern UI/UX**: Beautiful, responsive design with smooth animations
- 🔍 **Search Functionality**: Real-time search across all employee fields
- 📱 **Mobile Responsive**: Works perfectly on all device sizes
- ⚡ **Fast Performance**: Optimized for quick loading and smooth interactions
- 🛡️ **Data Validation**: Comprehensive form validation and error handling
- 🔔 **Notifications**: Real-time success/error notifications
- 🎨 **Beautiful Design**: Modern gradient backgrounds and card-based layout

## Tech Stack

- **Backend**: Node.js with Express.js
- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **Styling**: Custom CSS with modern design principles
- **Icons**: Font Awesome
- **Fonts**: Inter (Google Fonts)

## Prerequisites

Before running this application, make sure you have:

- Node.js (version 14 or higher)
- npm (comes with Node.js)

## Installation

1. **Navigate to the project directory**:
   ```bash
   cd project
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the application**:
   ```bash
   npm start
   ```

   Or for development with auto-restart:
   ```bash
   npm run dev
   ```

4. **Open your browser** and go to:
   ```
   http://localhost:3000
   ```

## API Endpoints

The application provides the following REST API endpoints:

- `GET /api/employees` - Get all employees
- `GET /api/employees/:id` - Get a specific employee
- `POST /api/employees` - Create a new employee
- `PUT /api/employees/:id` - Update an existing employee
- `DELETE /api/employees/:id` - Delete an employee

## Usage

### Adding an Employee
1. Click the "Add New Employee" button
2. Fill in all required fields:
   - Full Name
   - Email
   - Position
   - Department
   - Salary
   - Hire Date
3. Click "Save Employee"

### Editing an Employee
1. Click the "Edit" button on any employee card
2. Modify the information in the form
3. Click "Save Employee"

### Deleting an Employee
1. Click the "Delete" button on any employee card
2. Confirm the deletion in the popup dialog

### Searching Employees
- Use the search bar to filter employees by name, email, position, or department
- Search is performed in real-time as you type

## Employee Data Structure

Each employee record contains:
- **ID**: Unique identifier (auto-generated)
- **Name**: Full name of the employee
- **Email**: Email address
- **Position**: Job title/position
- **Department**: Department assignment
- **Salary**: Annual salary (numeric)
- **Hire Date**: Date when employee was hired

## Features in Detail

### Responsive Design
- Adapts to desktop, tablet, and mobile screens
- Touch-friendly interface for mobile devices
- Optimized layouts for different screen sizes

### Search Functionality
- Real-time search across multiple fields
- Case-insensitive matching
- Instant results as you type

### Form Validation
- Required field validation
- Email format validation
- Salary must be a positive number
- Date validation for hire date

### User Experience
- Loading spinners for async operations
- Success/error notifications
- Smooth animations and transitions
- Modal dialogs for forms and confirmations

### Data Persistence
- In-memory storage (for demo purposes)
- RESTful API design
- Proper error handling

## Customization

### Adding New Departments
To add new departments, edit the `department` select options in `public/index.html`:

```html
<option value="New Department">New Department</option>
```

### Styling Changes
The application uses custom CSS in `public/styles.css`. You can modify:
- Color scheme
- Typography
- Layout spacing
- Animation effects

### Backend Modifications
The server logic is in `server.js`. You can:
- Add database integration
- Implement authentication
- Add more API endpoints
- Enhance validation rules

## Troubleshooting

### Common Issues

1. **Port already in use**:
   - Change the port in `server.js` (line 8)
   - Or kill the process using the port

2. **Dependencies not installed**:
   - Run `npm install` again
   - Check if Node.js is properly installed

3. **CORS issues** (if accessing from different domain):
   - The server is configured with CORS enabled
   - Check browser console for any CORS errors

### Performance Tips

- The application uses in-memory storage for demo purposes
- For production, consider adding a database
- Implement pagination for large datasets
- Add caching for better performance

## Future Enhancements

Potential improvements for the application:

- [ ] Database integration (MongoDB, PostgreSQL)
- [ ] User authentication and authorization
- [ ] File upload for employee photos
- [ ] Export functionality (PDF, Excel)
- [ ] Advanced filtering and sorting
- [ ] Bulk operations
- [ ] Audit logging
- [ ] Email notifications
- [ ] Dashboard with analytics
- [ ] API rate limiting

## License

This project is open source and available under the MIT License.

## Support

If you encounter any issues or have questions, please check the troubleshooting section above or create an issue in the project repository. 