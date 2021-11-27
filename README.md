# SimRa-Visualization

This project is part of the SimRa research project which includes the following subprojects:
- [sirma-android](https://github.com/simra-project/simra-android/): The SimRa app for Android.
- [simra-ios](https://github.com/simra-project/simra-ios): The SimRa app for iOS.
- [backend](https://github.com/simra-project/backend): The SimRa backend software.
- [dataset](https://github.com/simra-project/dataset): Result data from the SimRa project.
- [screenshots](https://github.com/simra-project/screenshots): Screenshots of both the iOS and Android app.
- [SimRa-Visualization](https://github.com/simra-project/SimRa-Visualization): Web application for visualizing the dataset.

In this project, we collect – with a strong focus on data protection and privacy – data on such near crashes to identify when and where bicyclists are especially at risk. We also aim to identify the main routes of bicycle traffic in Berlin. To obtain such data, we have developed a smartphone app that uses GPS information to track routes of bicyclists and the built-in acceleration sensors to pre-categorize near crashes. After their trip, users are asked to annotate and upload the collected data, pseudonymized per trip.
For more information see [our website](https://www.digital-future.berlin/en/research/projects/simra/).


## Configuration / Install

1. Copy a gzip-ed database to `database/simra.sql.gz`
2. (Optionally) change ports in `docker-compose.yml``
3. Run `docker-compose up -d`. This might take forever and even afterwards you need to wait until the database is fully imported.
4. Setup the frontend so that it uses these services (`.env` in the frontend project)
