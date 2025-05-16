 User ||--o{ Property : owns
A User (specifically a host) can own zero or more Property entries.

Each Property is owned by exactly one User.

This relationship connects Property.host_id → User.user_id.

Interpretation:

A host (user) may own multiple properties, but a property belongs to only one host.

📅 User ||--o{ Booking : makes
A User (specifically a guest) can make multiple bookings.

Each Booking is linked to one user.

Interpretation:

A guest can book many properties, but each booking is made by a single user.

✍️ User ||--o{ Review : writes
A User (guest) can write multiple reviews.

Each Review is written by exactly one user.

Interpretation:

A guest can leave multiple reviews, but each review has only one author.

💬 User ||--o{ Message : sends
A User can send multiple messages.

Each Message is sent by exactly one sender.

📥 User ||--o{ Message : receives
A User can receive multiple messages.

Each Message is sent to exactly one recipient.

Interpretation:

Users can send and receive messages between each other.

🏘️ Property ||--o{ Booking : has
A Property can be booked multiple times.

Each Booking is for one specific property.

Interpretation:

A property can have many bookings, but each booking is for one property.

⭐ Property ||--o{ Review : receives
A Property can receive many reviews.

Each Review is written for one property.

Interpretation:

Guests can leave multiple reviews for a property.

💳 Booking ||--|| Payment : paid_by
Each Booking is associated with exactly one Payment.

Each Payment corresponds to one Booking.

Interpretation:

Every booking has one payment, and each payment pays for one booking.


