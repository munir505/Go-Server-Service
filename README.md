# Go-Server-Service
Make new user, in this case its called munir but can be changed in the service file (sudo useradd munir)

In order to run, first run Makefile command (sudo make) or (sudo make systemd_install)
Then run go-http-server.service file, (sudo service go-http-server.service start)
Then open up port 3000

if you ssh tunnel in to the VM then you can run (localhost:3000) in the browser, but would need to change proxy settings in browser

To uninstall, first do stop service (sudo service go-http-server.service stop)
Then uninstall via Makefile (sudo make systemd_uninstall)
