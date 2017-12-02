Convenience python class to provide communication between two udp speakers.
Provides useful defaults to make it easier.    Does not do a great job
with error recovery.

>>> import udp_channels as udp

>>> chan = udp.UDPChannel('192.168.1.176', 8888, '192.168.1.177', 8888)

>>> chan.send_to("hello to you")

>>> chan.receive_reply()

"hello yourself"
