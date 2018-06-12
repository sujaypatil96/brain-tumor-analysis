# Scalable and Efficient Genomic Data Store

### Title
Full-stack application for efficient storage and retrieval of large-scale clinical and genomic data for brain tumors.

### Introduction
For any contemporary clinical research, it is important to have clinical data about samples that are used in research along with large-scale molecular data. It is also essential to integrate in-house data with publicly available data. The final objective of the project is to collate glioma datasets primarily omics and other clinical data that are publicly available with some in-house generated datasets. It is important to store this big data in a format that allows for fast querying which makes relational databases a poor choice. The goal of this project will be to develop a clinical and genomic database for efficient storage and retrieval using NoSQL databases like MongoDB (which is a document store).

### Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

#### Prerequisites
Technology Stack

| System (s/w)  | Description       | Version|
| ------------- |:-----------------:|-------:|
| Apache        | Web Server        |  2.4   |
| PHP           | Application Layer |  5.4+  |
| Search Engine | Elasticsearch     |  2.4   |
| MongoDB       | Database Layer    |  3.4   |

* If you are on a Windows machine, you can consider installing the XAMPP technology stack.

*Note:* Find the XAMPP stack for Windows download [link here](https://www.apachefriends.org/index.html).

* There are some changes that need to be made in the `httpd.conf` file for Apache in order to integrate it with MongoDB.
* You need to download the appropriate driver for your version of XAMPP and copy the .dll file to XAMPP.
* Register mongo .dll file within `php.ini`, by adding the following line **extension=php_mongodb.dll**.
* To test if it worked — Restart XAMPP and refresh phpinfo.php page.
Note: Find detailed instructions to perform the above in the [link here](https://learnedia.com/install-mongodb-configure-php-xampp-windows/).

#### Installing and Running
* If the above steps worked, then you need to naviagte to the index.php page within the landing source files folder and find
the tabs you can navigate to there. To explain this in detail:

1. If you have followed the default the default instructions while installing XAMPP, you will find it installed at this location on your machine — `C:\xampp`.
2. Within this folder you will find an `htdocs` folder you will need to navigate to.
3. That is where you need to clone this repository to, or unzip the files.

* Open the XAMPP control panel, and turn on the Apache web server.
* At the same time, also navigate to where you installed MongoDB on your system. Fire up an instance of MongoDB by running the command  `mongod.exe` or just `mongod`.

*Note:* You will find the JSON file which needs to be imported into imported into your database in the project folder. Create a MongoDB database first, create within it a collection and import the JSON file directly into the collection.

* Now assuming you have followed all the steps as mentioned above, open any browser of your choice and type in the following URL (main_processing.php) — `http://localhost/DemoProject/Brain_Tumor_Analysis/public/main_processing.php`. Depending on the resources of your machine, it will take about 4 - 5 mins to execute the script.
* Then run the process_arrays.php script immediately after `http://localhost/DemoProject/Brain_Tumor_Analysis/public/process_arrays.php`.
* When both of these are finished running, you can then naviagte to the `index.html` page within the landing folder and play around with all the options built into the application.

### Existing Features
:TODO

### New Features
:TODO
