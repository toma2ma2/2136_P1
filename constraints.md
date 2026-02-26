| Description | Attribute(s) Involved | Constraint Category |
|------------------------|----------------------|--------------------------|
| number_of_hotels > 1 | number_of_hotels | Attribute Constraint (CHECK) or Derived Attribute |
| Each hotel must have exactly 1 manager | manager_employee_id | User-Defined Constraint |S
| manager_employee_id is unique | manager_employee_id | Key Constraint |
| manager_employee_id references Employee | manager_employee_id | Referential Integrity Constraint |
| star_rating must be between 1 and 5 | star_rating | Domain Constraint |
| room_capacity is single or double (between 1 and 2) | room_capacity | Domain Constraint |
| A customer can't create overlapping bookings for the same time period | customer_id, start_date, end_date | User-Defined Constraint |
| status must be ACTIVE, CANCELLED, or CONVERTED | status | Domain Constraint |
| booking_id is NULL for walk-in renting | booking_id | Attribute + Referential Integrity Constraint |
| employee_id in Renting cannot be NULL and must reference Employee | employee_id | Attribute + Referential Integrity Constraint |
| Hotel must have atleast 1 room | N/A | Domain Constraint| 