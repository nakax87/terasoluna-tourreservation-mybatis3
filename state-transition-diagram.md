# State Transition Diagram

```mermaid
stateDiagram-v2
    [*] --> Login
    Login --> SearchTour
    SearchTour --> TourDetails
    TourDetails --> ReserveTour
    ReserveTour --> ConfirmReservation
    ConfirmReservation --> Payment
    Payment --> [*]
    Payment --> CancelReservation
    CancelReservation --> [*]
    CancelReservation --> SearchTour
    ConfirmReservation --> CancelReservation
    ReserveTour --> CancelReservation
    TourDetails --> CancelReservation
    SearchTour --> CancelReservation
    Login --> CancelReservation
```
