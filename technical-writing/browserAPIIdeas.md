- Less used browser features
  - The Web Authentication API
    - Head
      - Good for mobile users
      - Easier login
      - WebAuthn built in to browser
      - Use Github webauthn-json library (easier)
    - Heart
      - Frustrating to type username/password on mobile
    - You
      - ???
  - Background Sync
    - Head
      - Good for when users lose connections
      - Retries failed network requests
      - Works in service worker
      - Example use case: on the subway
      - Uses retry queue
    - Heart
      - Frustration of losing data
      - Can improve confiudence in system
    - You
      - ???
  - The Cache API
    - Head
      - Local storage of files
      - Can use caching strategies
      - Works well with service workers
      - Improve loading performance
      - Use when offline
    - Heart
      - Happy when bandwidth usage lower
      - Frustrated when pages load slowly
    - You
      - Security issue if confidential data stored
  - The Beacon API
    - Head
      - Save data at end of session
      - Useful for analytics data
      - Called sendBeacon instead of fetch
      - Guaranteed to complete
      - Will work even if user leaves the page
      - can track end of session
    - Heart
      - Relief if did not save data
    - You
      - ???
    - The Web Socket API
        - Head
             - Open connection to server
             - Code in client and server
             - Server can notify client

        - Heart

             - Happy that data up to date

        - You

             - Attackers might soak server resources

    - Background Fetch
        - Head
             - Download files in background
             - Can use service worker
             - Send notification when complete
             - With caches can use files offline

        - Heart

             - Do not have to worry about constant network coverage

        - You

             - Must be responsible and not start too many downloads

             - Should make user aware that download is running and when complete

    - Online/offline detection
        - Head
             - Notice when network disappears
             - "Online" does not necessarily mean connected to the Internet
             - Can disable UI if requires network connection

        - Heart

             - Avoid disappointing user by disabling UI

        - You

             - Should use alongside other services (e.g. CatchHandlers)

    - The Web Speech API
        - Head
             - Text to speech
             - Available in a lot of browsers

        - Heart

             - Could be irritating if user hasn't enabled it

        - You

             - Useful because should check UI with some sort of screen reader

    - Two-Factor Authentication
        - Head
             - Users
             - Security
             - Use anywhere
             - USB token
             - Uses WebAuthn

        - Heart

             - Increased confidence

        - You

             - User must choose to opt in

             - Other attack vectors

                 - Social engineering

                     - Phone up and claim you lost the token

    - Catch Handler
        - Head
             - Handle failed network requests in service worker
             - Can send back alternative resources from cache
             - Can check how the request was made
             - Can still show errors if needed

        - Heart

             - Nicer experience to smoothly downgrade UI

        - You

             - ???

    - Vibration API
        - Head
             - Make a mobile device vibrate
             - Requires special permissions

        - Heart

             - Could be really irritating

        - You

             - Overuse might drain the battery

    - Location Sensor API
        - Head
             - Find lat/long use GPS or Wifi

        - Heart

             - Increased ease of use for location-specific data

        - You

             - Potential for misuse of data

             - Security flaws if store data without needing to

             - Use might contravene local laws

    - Accelerometer
        - Head
            - Tracks movement of the device
            - Many practical uses?

        - Heart

            - ???

        - You

            - ???
