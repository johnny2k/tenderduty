# Matrix Configutation

To push messages to a Matrix channel you need the internal room ID and an access token for a user.

This example uses the Element Matrix client.

* Find the "Internal room ID"
 - Room info icon -> Settings -> Advanced

* Obtain your user access token

 - Open Element Settings
 - Click Help & About
 - At the bottom, under Advanced, click Access Token
 - Copy your token

* Configure in config.yml or in chain specific settings.

``` 
    # Matrix settings
    matrix:
      # Send alerts to Matrix?
      enabled: yes 
      room_url: https://HOME_SERVER/_matrix/client/r0/rooms/INTERNAL_ROOM_ID/send/m.room.message/?access_token=ACCESS_TOKEN
```

The room_url will look something like this...
    https://matrix.org/_matrix/client/r0/rooms/!iItOTalLymaDEthIsup:matrix.org/send/m.room.message/?access_token=tHiStokeNisNTreaLbuTmaYbEitlOoKsReAlenouGhaSaNExampLe
