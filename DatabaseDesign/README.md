# Gym Membership

 This simple database manages the gym membership.
 
## Use cases
   - Each member has a unique ID, a name, email and a phone number
   - Each member must only have 1 membership at a time. Member's info can be kept even when the membership expired
   - The membership must have a start date or end date
   - Every member must reserve a schedule spot to get access to the gym.
   - Any member can optionally ask for a coach for the reserved schedule
   
## List of entities

  **Member**:
   - MemberID (PK)
   - FirstName
   - LastName
   - Email
   - PhoneNumber
  
  **Membership**:
   - MembershipID (PK)
   - DateStart
   - DateEnd
   - MembershipFee
  
  **Staff**
   - StaffID (PK)
   - FirstName
   - LastName
   - Email
   - PhoneNumber
   - IsACoach
  
  **Schedule**
   - ScheduleID (PK)
   - Date
   - GymRoom
   - MemberID (FK)
   - StaffID (FK)
