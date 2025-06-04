# DG Shoes - Ecommerce Website

A full-featured ecommerce web application for shoes built with Django, following the Model-View-Template (MVT) architecture.

## Features

- **Product Management**: Browse and search shoe collections
- **User Authentication**: User registration, login, and profile management
- **Shopping Cart**: Add, remove, and update items in cart
- **Order Management**: Place orders and track order history
- **Payment Integration**: Secure payment processing with Razorpay
- **Admin Panel**: Django admin interface for managing products, orders, and users
- **Responsive Design**: Mobile-friendly interface using Django templates

## Tech Stack

- **Backend**: Django (Python)
- **Frontend**: Django Templates, HTML, CSS, JavaScript
- **Database**: PostgreSQL
- **Payment Gateway**: Razorpay
- **Architecture**: Model-View-Template (MVT)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Sidharth-Chirathazha/DG-SHOES-ECOMMERCE.git
   cd dg-shoes
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Setup**
   Create a `.env` file in the root directory:
   ```env
    SECRET_KEY=YOUR SECRET KEY
    DB_ENGINE=YOUR DB ENGINE
    DB_NAME=YOUR DB NAME
    DB_USER=YOUR DB USERNAME
    DB_PASSWORD=YOUR DB PASSWORD
    DB_HOST=YOUR DB HOST
    DB_PORT=YOUR DB PORT
    EMAIL_BACKEND=YOUR EMAIL BACEKND
    EMAIL_HOST=YOUR EMAIL HOST
    EMAIL_USE_TLS=TRUE/FALSE
    EMAIL_PORT=YOUR EMAIL PORT
    EMAIL_HOST_USER=YOUR EMAIL HOST USER
    EMAIL_HOST_PASSWORD=YOUR EMAIL HOST PASSWORD
    EMAIL_USE_SSL=TRUE/FALSE
    RAZORPAY_KEY_ID=YOUR RAZOR PAY KEY ID
    RAZORPAY_KEY_SECRET=YOUR RAZOR PAY KEY SECRET
   ```

5. **Database Setup**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create Superuser**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the Application**
   ```bash
   python manage.py runserver
   ```

The application will be available at `http://localhost:8000`

## Configuration

### Razorpay Setup
1. Sign up at [Razorpay](https://razorpay.com/)
2. Get your API keys from the dashboard
3. Add the keys to your `.env` file
4. Configure webhook URLs for payment confirmation

### Static Files
For production deployment:
```bash
python manage.py collectstatic
```


## Usage

1. **Admin Access**: Visit `/admin_login` to manage products and orders
2. **User Registration**: Users can create accounts and manage profiles
3. **Shopping**: Browse products, add to cart, and checkout
4. **Payment**: Secure payment processing through Razorpay
5. **Order Tracking**: Users can view their order history


## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## Deployment

For production deployment:

1. Set `DEBUG=False` in settings
2. Configure allowed hosts
3. Set up a production database (PostgreSQL recommended)
4. Configure static file serving
5. Set up SSL certificates
6. Use a production WSGI server (Gunicorn)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support and questions, please open an issue in the GitHub repository.

---

**DG Shoes** - Your trusted online shoe store
