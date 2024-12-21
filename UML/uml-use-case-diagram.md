# UML Use Case Diagram

```mermaid

graph TB
    User((User))
    Admin((Admin))
    Secretary((Secretary))
    ITOfficer((IT Officer))
    Driver((Driver))
    
    subgraph DriverPass System
    Login[Login]
    ManageAccount[Manage Account]
    ResetPassword[Reset Password]
    BookLesson[Book Driving Lesson]
    ModifyBooking[Modify Booking]
    TakeTest[Take Practice Test]
    ViewProgress[View Progress]
    ManageUsers[Manage Users]
    GenerateReports[Generate Reports]
    ManagePackages[Manage Packages]
    ManageDrivers[Manage Drivers]
    TrackVehicles[Track Vehicles]
    UpdateDMV[Update DMV Content]
    end
    
    User --> Login
    User --> ResetPassword
    User --> BookLesson
    User --> ModifyBooking
    User --> TakeTest
    User --> ViewProgress
    
    Admin --> Login
    Admin --> ManageUsers
    Admin --> GenerateReports
    Admin --> ManagePackages
    
    Secretary --> Login
    Secretary --> BookLesson
    Secretary --> ModifyBooking
    
    ITOfficer --> Login
    ITOfficer --> ManageUsers
    ITOfficer --> UpdateDMV
    
    Driver --> Login
    Driver --> ViewProgress
    Driver --> ManageDrivers

    ```