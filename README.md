# cups for raspberrypi

# cups admin=pi pass=pi

docker run -d --name="cups4rpi" --net="host" --privileged="true" --restart always 
-v /var/run/dbus:/var/run/dbus -v /dev/bus/usb:/dev/bus/usb -v /dev:/dev rabbired/cups4rpi
