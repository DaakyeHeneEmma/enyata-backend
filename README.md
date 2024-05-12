# enyata-backend

# The required working flow:

    A POST endpoint that receives the incident report.

The report should have the following data :

{ “client_id”: number, “incident_desc: string, “city”: string, “country”: string }

The endpoint receives the report, adds weather data and stores it in a table “incidents”.

The weather report should be fetched from the API service of https://openweathermap.org/current

# The stored object should be then as follow:

{ “client_id”: number, “incident_desc: string, “city”: string, “country”: string, “date”: date, “weather_report”: object }

    A GET endpoint that lists all the incidents.

# The endpoint should have the capability of filtering the data by city, temperature range and humidity range.

    A POST endpoint that searches for incidents based on country name.

    Write integration tests (and unit tests if applicable) of all endpoints.


# Stack:

    NodeJS and express (required)

    PostgreSQL (required)

    ORM: Sequelize (optional)

    Mocha (required)

    Chai (required)