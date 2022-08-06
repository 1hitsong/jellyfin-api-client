This library is meant to help clients written in Brightscript interact with Jellyfin's REST API.

All API Helper Functions copied from Jellyfin Roku https://github.com/jellyfin/jellyfin-roku

## Config
Communication with the Jellyfin API relies on 3 configuration variables:

1. APIKEY
2. SERVERURL
3. ACTIVEUSER

To pass these values into the API, you must create 2 functions:

1. get_user_setting(name AS string)
2. get_setting(name AS STRING)

Your functions need to accept a name parameter and return the correct value, as seen below.

    APIKEY: get_user_setting("token")

    ACTIVEUSER: get_setting("active_user")

    SERVERURL: get_setting("server")