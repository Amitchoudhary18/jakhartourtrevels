JAKHAR TOUR TRAVELS - LATEST FIX

1) index.html = customer page
2) admin.html = admin page
3) driver.html = driver page
4) FIRESTORE_RULES.txt = testing rules; publish these in Firebase Firestore Rules

FIXES:
- Admin page no longer displays the temporary PIN text.
- Vehicle Photos & Interior Gallery section removed from Admin.
- Admin driver Reset Password now has proper error handling.
- Admin driver Remove button now has proper error handling and success confirmation.
- Driver ON/OFF Duty uses Firestore set(...,{merge:true}) and shows the actual Firebase error if it fails.
- Driver ON Duty plays a short browser sound from the button click.
- Driver live location now sends an immediate GPS position with getCurrentPosition and also keeps watchPosition active.
- Manual Update Live Location button forces a location update.
- Location permission/GPS errors are shown clearly.

IMPORTANT:
For Duty status, driver management, bookings, and fare saving to work, publish FIRESTORE_RULES.txt in the Firebase Console.
For live location, allow Location permission in the browser and keep GPS/location enabled on the device.
