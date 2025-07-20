# alx_travel_app_0x00

## Database Modeling and Seeding

This project implements a travel application with database models for listings, bookings, and reviews, along with API serializers and a seeder command.

### Models
- `Listing`: Represents a property with title, description, price, location, and capacity.
- `Booking`: Manages reservations with check-in/out dates and total price.
- `Review`: Stores user ratings and comments for listings.

### Serializers
- Defined in `listings/serializers.py` for API data representation of `Listing`, `Booking`, and `Review`.

### Seeder
- Use `python manage.py seed` to populate the database with sample data.
- Requires migrations to be applied first: `python manage.py makemigrations` and `python manage.py migrate`.

### Setup
1. Activate the virtual environment: `.\venv_messaging\Scripts\activate`
2. Apply migrations: `python manage.py migrate`
3. Seed the database: `python manage.py seed`