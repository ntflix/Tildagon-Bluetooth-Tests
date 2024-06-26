# TildaDrop

An example of using [ESP-NOW](https://docs.micropython.org/en/latest/library/espnow.html) to wirelessly and (relatively) hassle-freely send data between badges.

The MAC address of the target badge is needed on the 'sender' badge. Set this in the `PEER_MAC` variable in `app.py`.

You can find a board's MAC through pressing the `right` button of the Tildagon in this app.

Broadcast functionality, which does not require the MAC address of a recipient, does not seem to work as it shows in the [espnow docs](https://docs.micropython.org/en/latest/library/espnow.html#broadcast-and-multicast).

> Two badges are needed for this to work - a badge to send, a badge to receive.

1. On receiver badge, enter receiving mode in the app
2. On sender badge, hit sending mode
3. Receiver badge screen will turn white and (temperamentally) say "Received!" with the message data (default 'Hi').
