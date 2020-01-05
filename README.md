# 🔥 FireLocs

A project used during a 2020 [NCSS](https://ncss.edu.au/summer-school) masterclass, demonstrating a web service for [RFS](https://www.rfs.nsw.gov.au) bushfire data used. The masterclass is given by @goodtune and @edwinsteele

## Getting started

Create a `virtualenv` in which to install the project dependencies.

    virtualenv -p python3.7 venv

Install the dependencies with `pip`.

    venv/bin/pip install -r requirements.txt

Create your database.

    venv/bin/python manage.py migrate

Populate your database with demonstration incident data.

    venv/bin/python manage.py import_fires data/demonstration.xml

Start the development server.

    venv/bin/python manage.py runserver

Launch your browser and visit http://localhost:8000/ and http://localhost:8000/json/ to interact with the system.

## Loading Live RFS data (optional)

    venv/bin/python manage.py import_fires http://www.rfs.nsw.gov.au/feeds/majorIncidents.xml

## Slides

   <https://goodtune.github.io/firelocs>
