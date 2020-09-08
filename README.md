# Sakila ETL Workshop

Welcome!, this is my workshop to get to know how *Extraction*, *Tranformation* and *Load* operations work for business intelligence purposes. In here, we are using the Sakila sample database of MySQL as our data source, you can find more [here](https://dev.mysql.com/doc/sakila/en/).

## Running the data source on Docker

This project has automatized the database on a Docker instance, you just have to run this command on your local machine:

	docker-compose up -d

Wait for the MySQL instance and database to finish is initial load and connect to it with any Database Administration Software you want (For example, MySQL Workbench).

To connect to the database, use this values:

	Hostname: localhost or 127.0.0.1
	Port: 3306
	Username: root
	Password: secret

## Sakila database definition

Here you can find a diagram of the Sakila database with 16 tables between films, actors, customers, staff, stores and rentals of a DVD rental chain store. 

![alt text](./misc/Sakila_database.PNG "Database diagram")

## ETL operations requirements and definitions

1. Contrastar popularidad de las peliculas con bases de datos alternativas (Rotten Tomatoes, IMdb)

2. Total de películas no pagadas y pérdida de dinero

3. Géneros más vistos por ciudad, país, anualmente, mensualmente

4. Géneros más rentables por ciudad, país, anualmente, mensualmente

5. Relación entre rentabilidad y actor respecto a premiaciones

6. Rentabilidad por país y ciudad
