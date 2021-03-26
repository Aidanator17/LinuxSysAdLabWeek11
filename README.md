HOW TO INSTALL

make sure your working directory is where the downloaded files are
copy the ws.service and the ws.timer files to the directory /etc/systemd/system
commands to copy the files:
$ cp ws.service /etc/systemd/system
$ cp ws.timer /etc/systemd/system

copy the script file (ws) to the directory /home/vagrant/week11
(if the directory doesnt exist, either change the directory in the ws.service script or use mkdir)
$ cp ws /home/vagrant/week11

reload and start your service and timer files
commands to reload and start
$ sudo systemctl daemon-reload
$ sudo systemctl start ws.service
$ sudo systemctl start ws.timer

done! your weather script should be running hourly, check weather.txt in /home/vagrant/week11 for the output
