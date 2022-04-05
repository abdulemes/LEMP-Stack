# Project Workflow

## Phase 1 - Setting up a VM

Step 1 - Setup a virtual machine on oracle virtualbox using vagrant.

Step 2 - Go in the directory where the vagrantfile is and bring up the VM.

![IMG_9510](https://user-images.githubusercontent.com/93732510/161714607-507b3dd9-8d02-44a8-8bca-a53f97701958.jpg)

Step 3 - log into the VM using ssh

![IMG_9511](https://user-images.githubusercontent.com/93732510/161716896-02341ee5-4bdb-46dd-889a-897230dc5086.jpg)

## Pahse 2 - Installing NGINX web server

Step 1 - The package manager gets updated in this step.

![IMG_9512](https://user-images.githubusercontent.com/93732510/161718126-b7962207-4e9d-4161-af25-09b48f41a516.jpg)

Step 2 - The NGINX web server is then installed. 

![IMG_9514](https://user-images.githubusercontent.com/93732510/161718424-cfa0cb80-f5c4-4752-88e5-fc0739aa704d.jpg)

Step 3 - Its essential to check that the server is successfully installed and running. 

![IMG_9515](https://user-images.githubusercontent.com/93732510/161718964-31f96bae-f577-4ca3-b1ad-c65edb369b68.jpg)

Step 4 - Next is to confirm via the browser if the server can be accessed.

![IMG_9516](https://user-images.githubusercontent.com/93732510/161719312-c00ed1a2-d65b-440f-b070-9125f44f6274.jpg)

## Phase 3 - Installing MYSQL

Step 1 - MYSQL database is installed.

![IMG_9517](https://user-images.githubusercontent.com/93732510/161719636-b376cf7b-b21a-47b8-b708-eee04b16c742.jpg)

Step 2 - Security script to remove insecure default settings is being run.

![IMG_9518](https://user-images.githubusercontent.com/93732510/161720144-745df872-572d-40a3-854d-b910fbad2f8c.jpg)

Step 3 - logging in to mysql as a root user to test the mysql server.

![IMG_9519](https://user-images.githubusercontent.com/93732510/161720861-d44e37fc-f603-4fcc-996d-17517a9546b7.jpg)

## Phase 4 - Installing PHP

Step 1 - This step is where php process manager gets installed along with php mysql module.

![IMG_9520](https://user-images.githubusercontent.com/93732510/161721810-b85348aa-dd2c-4f21-af53-1b3831780c1b.jpg)

## Phase 5 - Configuring NGINX to use PHP processor

Step 1 - A root web directory is created for the domain and ownership is assigned. 

![IMG_9521](https://user-images.githubusercontent.com/93732510/161723312-c3eca3d0-7102-4ec8-9053-9bee6a52ea5a.jpg)

Step 2 - Next is to setup configuration file in NGINX sites-available directory using vim editor.

![IMG_9522](https://user-images.githubusercontent.com/93732510/161726185-4ec5a9da-f825-4eba-b02f-401d6851f949.jpg)

Step 3 - Activating the configuration by linking it to NGINX ites enabled directory, testing to see if the sysntax is ok.

![IMG_9524](https://user-images.githubusercontent.com/93732510/161727325-bef04e2b-1173-4ba2-8ac8-352342389e3d.jpg)

Step 4 - Next is to unlink the default NGINX host, reload NGINX for changes to take effect and create an index.html file to test the website.

![IMG_9530](https://user-images.githubusercontent.com/93732510/161728310-ee8c1cf4-9797-4c0a-91e9-7318b3590134.jpg)

Step 5 - Checking the output via the browser. 

![IMG_9531](https://user-images.githubusercontent.com/93732510/161728551-2f043c67-a0f9-45e7-b6c5-bcd077bdbec3.jpg)

## Phase 6 - Testing PHP with NGINX

Step 1 - Creating a php file at server directory using vim editor.

![IMG_9533](https://user-images.githubusercontent.com/93732510/161729233-ca22cda5-bb56-4eff-b97c-f1e23b6c8a5b.jpg)

Step 2 - Verifying that the php file is successfully served to the browser.

![IMG_9538](https://user-images.githubusercontent.com/93732510/161729498-a002bed2-abba-43fc-a3e1-21aba4b837a0.jpg)

## Retrieving data from mysql databse with php

Step 1 - First thing is to connect to the mysql console using root account

Command : sudo mysql

Step 2 - A sample database is created, a user that will access the database is created, and necessary permission is assigned. 

![IMG_9539](https://user-images.githubusercontent.com/93732510/161730611-3b50b189-2d8b-4eea-9f3e-9931243f11fd.jpg)

Step 3 - we log in to mysql using the credentials of the new user created. 

![IMG_9540](https://user-images.githubusercontent.com/93732510/161730890-d04a0689-a708-4a8a-a082-07acac4d594a.jpg)

Step 4 -  Here, the user is able to request the sample database created and a sample table is created as well. 

![IMG_9543](https://user-images.githubusercontent.com/93732510/161732455-c04f55f5-b6c7-49ea-bc58-9d5a988dce26.jpg)

Step 5 - After the table is created, a few rows are inserted in the table and then queried to see the output.

![IMG_9544](https://user-images.githubusercontent.com/93732510/161732866-af07c482-02df-4430-8120-a6027f8b7fc7.jpg)

Step 6 - Next is to create a php script that will connect to mysql in web root directory using vim editor.

![IMG_9545](https://user-images.githubusercontent.com/93732510/161733487-8928455d-bdf3-44bf-8a56-bcd64a80eb1c.jpg)

Step 7 - Now we can check that the php file is served to the browser.

![IMG_9546](https://user-images.githubusercontent.com/93732510/161733893-b58dc6c2-fbb8-427d-a03a-3629f7e3b785.jpg)












