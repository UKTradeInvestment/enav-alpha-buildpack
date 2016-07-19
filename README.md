# enav-alpha-buildpack
The heroku buildpack for the enav-alpha application

enav-alpha buildpack to run the necessary installation of the enav-alpha application the heroku infrastructure.  

## Setup

1. Set Heroku's default Python buildpack for your app, set up Python and install the required python dependencies.

    ```bash
    heroku buildpacks:set https://github.com/heroku/heroku-buildpack-python
    ```

2. Set Heroku's default NodeJS buildpack for your app, set up NodeJS. 

    ```bash
    heroku buildpacks:add https://github.com/heroku/heroku-buildpack-nodejs
    ```

3. Add this buildpack, build the static assets used by the system.

    ```bash
    heroku buildpacks:add https://github.com/UKTradeInvestment/enav-alpha-buildpack.git
    ```
