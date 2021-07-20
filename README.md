# xdocker-apps
Definitions of some xdocker apps

## Howto

Just build the images (eg. `docker build -t xdocker-(app-name) .`) and copy the xdocker file as `$HOME/.config/xdocker/(app-name)`

## Special cases

* OBS and Qutebrowser uses hardware video acceleration, with only the intel va-api driver installed, if you have an AMD or nvidia card, you need to install the correct package
* ghidra is launched for 8G of memory, adjust if needed
* you'll need to provide your own chitubox zip (after registration, so no automatically downloadable)
