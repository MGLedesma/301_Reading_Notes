# RADIUS

Resource: [RADIUS Concepts](https://wiki.freeradius.org/guide/Concepts)

Remote Authentication Dial-In User Service (802.1X)
- a client/server protocol
- is a networking protocol that uses the provision of AAA - Authentication, Authorization, and Accounting - and its part of the IEEE 802.1X security standard.
    - Authentication and Authorization happens simultaneously - device creates a message called an Access-Request message and sends it to the RADIUS server. A username and password. The RADIUS server uses an allowed authentication method and looks for a match in its database, if a configuration policy is found, it accepts the request by sending a response. If the request is rejected the transaction ends and the user is denied access.
    - Accounting - the server collects data for statistical purposes and network monitoring. Once access has been granted NAS sends a RADIUS Accounting Request packets
        - Accounting Start - contains user's ID, unique session identifier, point of access and network address)
        - Interim Update - consits of session duration and current date usage
        - Accounting Stop Record - provides comprehensive session information, once the user access to the RADIUS server has ceased.
    - Finally, the RADIUS server responds with an Accounting Responce acknowledgement - the accounting process of a particular user is complete and all information related to the session is stored in the server.
