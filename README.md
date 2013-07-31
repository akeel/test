I am a developer myself, but I am looking for a Ruby on Rails expert to assist me in creating a simple Restaurant Booking System. I am trying to form a long term relationship as I have other businesses that are also built on RoR.

I am open to suggestions, but my thoughts so far are

1) a private website for users using Devise and Omni Auth (to use facebook/google authentication) that will allow users to login and make reservations, and also view their booking history
2) a private website for Restaurant owners to manage the available inventory

NO DESIGN is needed, just need the programming functionality

The models should be as follows (unless suggested otherwise)

Users:
-email
-name
-phone

Restaurants:
-name
-type/catagory
-lat-longitude (for google maps integration)
-Text Field (for misc information)

Reservations:
-belongs to: user
-belongs to: restaurant
-start-time
-end-time
-party size
-active:boolean

Inventory:
-date
-00:00-23:45 (everytime from 00:00 to 24:00 in 15 minute increments)
-quantity available

Defaults:
-name
-00:00-23:45 (everytime from 00:00 to 24:00 in 15 minute increments)
-quantity available
-primary:boolean


User will login, and search for available inventory based on existing, active reservations in the system and the "inventory" defined in the inventory table. They should be able to login and check/cancel a booking
