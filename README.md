# SNA-LGTC boot scripts

These are boot scripts that reside in `/opt/scripts` on the SNA-LGTC board.
They are a modified version of the scripts that ship with the original SD card
images for BeagleBone boards.

They get called from various places (such as systemd services) after boot and
perform hardware initialization tasks (such as bringing up the Wireless
network, USB network interface and so on). These scripts also include the eMMC
flasher that copies the content of the SD card to the internal eMMC flash.

They are not packaged into Debian packages (although some things that *are*
packaged by BeagleBone may depend on these scripts). Rather, this repository is
simply checked out into `/opt/scripts` on the original SD card images.

See also the [sna-lgtc-support](https://github.com/sensorlab/sna-lgtc-support)
repository.
