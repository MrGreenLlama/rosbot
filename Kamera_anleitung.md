Kamera über ROS übertragen
===
---
Die ganzen Kamera-modi anzeigen:

    v4l2-ctl --list-formats-ext
<br>
Diese tolle Datei hat der Professor für uns hinterlassen, in ihr kann man Kameraeinstellungen umstellen:


    nano ~/catkin_ws/libuvc_camera.launch

einfach die Parameter der modi von vorher in die Datei reinfüllen:

z.b.:
>\<param name="frame_rate" value="30"/>

wird zu

>\<param name="frame_rate" value="25"/>

<br>

das Skript dann ausführen:

    roslaunch libuvc_camera.launch

>oder in einen screen packen  
> z.B.: `screen -S camera roslaunch libuvc_camera.launch`

>Ich hab LEIDER noch kein skript dafür ~~Werbung~~