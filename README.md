Update: Moved to [Gitlab](https://gitlab.com/eschabell/chapter-8-form-design-demo).


Chapter 8 - Form Design Demo 
=============================
This is an example project for the Effective Business Process Management with JBoss BPM book, 
used in chapter 8. It is a project to automate the installation of the product JBoss BPM Suite 
with preconfigured admin user and sane project defaults.


Option 1 - Install on your machine
----------------------------------
1. [Download and unzip.](https://github.com/effectivebpmwithjbossbpm/chapter-8-form-design-demo/archive/master.zip)

2. Download JBoss EAP & JBoss BPM Suite, add to installs directory (see installs/README).

3. Run 'init.sh' or 'init.bat' file. 'init.bat' must be run with Administrative privileges. 

4. Login to http://localhost:8080/business-central  (u:erics / p:bpmsuite1!)

5. Enjoy installed and configured JBoss BPM Suite.


Option 2 - Generate containerized installation
----------------------------------------------
The following steps can be used to configure and run the demo in a container

1. [Download and unzip.](https://github.com/effectivebpmwithjbossbpm/chapter-8-form-design-demo/archive/master.zip)

2. Download JBoss EAP & JBoss BPM Suite, add to installs directory (see installs/README).

3. Build demo image.

	```
	docker build -t effectivebpmwithjbossbpm/chapter-8-form-design-demo .
	```
4. Start demo container

	```
	docker run -it -p 8080:8080 -p 9990:9990 -p 8001:8001 effectivebpmwithjbossbpm/chapter-form-design-demo
	```

Login to http://localhost:8080/business-central (u:erics / p:bpmsuite1!) 

Released versions
-----------------
See the tagged releases for the following versions of the product:

- v1.0 - JBoss BPM Suite 6.4.0 installed on JBoss EAP 7.0.0 and optional containerized install.

![BPM Suite](https://raw.githubusercontent.com/effectivebpmwithjbossbpm/chapter-8-form-design-demo/master/docs/demo-images/bpmsuite.png)
