# Requirements

1. The system shall utilize a publish subscribe architecture.

1. The system shall use middleware based on the MQTT-protocol.

1. The system shall utilize a Publish/Subscribe system for the MQTT protocol.

1. The system shall allow users to book dentist appointments.

1. The system shall display a web-based GUI, which should include:
    1.  User specified time-slots.
    1. Track free time-slots and dentist availability.
    1. A confirmation/rejection notification.
    1. A map-view over Gothenburg that can be navigated.
    1. Allow for user requests.
    1. Delegate incoming user requests.
    1. Reactivity to booked user slots.

1. The system shall be a distributed system.

1. The system shall consist of at least 4 distributed components, which shall clearly contribute to the purpose of the application.

1. The system shall track free time slots and dentist availability.

1. The system shall send confirmation and rejection notifications to users.

1. The components shall be resistant to standard failures, out of bounds inputs and ill-formatted data inputs.

1. The components shall unsubscribe from the MQTT broker when stopped.

1. The system shall be able to communicate and utilize the dentist registry database.

1. The system shall contain time slots, which shall:
    1. Be 30 minutes in lenght,
    1. Include a one hour lunch break, as well as a 30 minute Swedish Fika break.

1. The booking requests shall follow a predefined format, that is handled through the MQTT-middleware.