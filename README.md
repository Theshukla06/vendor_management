# vendor_management
# Vendor Management System

This Django-based Vendor Management System allows you to manage vendor profiles, track purchase orders, and calculate vendor performance metrics.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Running Tests](#running-tests)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/vendor-management-system.git
cd vendor-management-system

2. Set up a virtual environment:
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3. Install dependencies:
pip install -r requirements.txt

4. Apply migrations:
python manage.py migrate

5. Create a superuser account:
python manage.py createsuperuser

6. Run the development server:
python manage.py runserver
Access the Django admin at http://localhost:8000/admin/ and log in with the superuser credentials.



API Endpoints
The following API endpoints are available:

Vendor Management:

POST /api/vendors/: Create a new vendor.
GET /api/vendors/: List all vendors.
GET /api/vendors/{vendor_id}/: Retrieve a specific vendor's details.
PUT /api/vendors/{vendor_id}/: Update a vendor's details.
DELETE /api/vendors/{vendor_id}/: Delete a vendor.
Purchase Order Tracking:

POST /api/purchase_orders/: Create a purchase order.
GET /api/purchase_orders/: List all purchase orders with an option to filter by vendor.
GET /api/purchase_orders/{po_id}/: Retrieve details of a specific purchase order.
PUT /api/purchase_orders/{po_id}/: Update a purchase order.
DELETE /api/purchase_orders/{po_id}/: Delete a purchase order.
Vendor Performance Evaluation:

GET /api/vendors/{vendor_id}/performance: Retrieve a vendor's performance metrics.
Update Acknowledgment:

POST /api/purchase_orders/{po_id}/acknowledge: Acknowledge a purchase order.

