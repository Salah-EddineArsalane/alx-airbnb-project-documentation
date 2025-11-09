# Airbnb Clone – Data Flow Diagram

This diagram illustrates how data flows through the system.

## Main Processes:
- **User Registration:** User inputs → validated → stored in User DB.
- **Property Management:** Host adds property → stored in Property DB.
- **Booking:** Guest books property → stored in Booking DB → triggers payment process.
- **Payment:** Payment info → verified via Stripe API → stored in Payment DB.

Refer to `data-flow.png` for the complete visual layout.
