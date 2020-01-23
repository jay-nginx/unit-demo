# unit-demo
This is my very basic Unit Demo.

For Ubuntu:

Check Status / Start / Stop
sudo systemctl status unit

What is running in your UNIT Instance:
sudo curl --unix-socket /var/run/control.unit.sock localhost/config

Apply new configuration / Deploy new App in UNIT:
sudo curl --unix-socket /var/run/control.unit.sock -X PUT --data-binary @/opt/unit/demo1/combined.config localhost/config
