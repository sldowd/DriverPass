# Book Driving Lesson Activity Diagram

```mermaid

stateDiagram-v2
    [*] --> Login
    Login --> SelectPackage
    SelectPackage --> ViewAvailableSlots
    ViewAvailableSlots --> SelectTimeSlot
    SelectTimeSlot --> EnterPickupLocation
    EnterPickupLocation --> ConfirmBooking
    ConfirmBooking --> ProcessPayment
    ProcessPayment --> Success
    ProcessPayment --> Failed: Payment Error
    Failed --> ViewAvailableSlots
    Success --> [*]

```