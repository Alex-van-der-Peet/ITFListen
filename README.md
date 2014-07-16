itf_listen
=======

itf_listen uses Google's speech-to-text API to convert a sound recording obtained using sox into a string representation

Usage
-------------
Clone into your catkin workspace, to run:

rosrun itf_listen itf_listen.py

Output will be published on the /itf_listen topic. If Google fails to recognize the voice input, the message BADINPUT will be posted instead.


Notes
-------------
If at any time Google decides to shutdown / switch API's (as was the reason for rewriting this to support the v2 API rather than the v1 API) this code will probably require some changes.
