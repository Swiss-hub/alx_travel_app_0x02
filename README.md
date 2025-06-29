# ALX Travel App

This Django app provides API endpoints for managing listings and bookings.

## Payment Integration

- Users can pay for bookings securely via Chapa.
- Payment workflow:
  1. Initiate payment: `/api/payments/initiate/<booking_id>/`
  2. Complete payment via Chapa checkout link.
  3. Verify payment: `/api/payments/verify/<tx_ref>/`
- Payment status is tracked in the Payment model.

## Endpoints

- `/api/listings/` - CRUD for listings
- `/api/bookings/` - CRUD for bookings
- `/api/payments/initiate/<booking_id>/` - Initiate payment for a booking
- `/api/payments/verify/<tx_ref>/` - Verify payment status

API documentation is available at `/swagger/`.
