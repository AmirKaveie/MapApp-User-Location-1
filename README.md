Location Permissions:

    The Location.requestForegroundPermissionsAsync() function requests permission to access the user's location while the app is in the foreground. If the user denies this permission, an alert is shown.

Fetching Current Location:

    Once the permission is granted, Location.getCurrentPositionAsync({}) fetches the current location of the user. The location data includes latitude and longitude.

State Management:

    useState is used to manage the user's location (location) and any potential error messages (errorMsg).

Rendering the Map:

    The MapView component is configured to initially center the map on the user's location if available. If the location isn't available yet (e.g., while waiting for permission), a default location is used.

User Location Marker:

    If the location is available, a Marker is placed on the map at the user's current location.

showsUserLocation:

    The showsUserLocation prop automatically displays a blue dot on the map at the user's location, which is a built-in feature of react-native-maps.
