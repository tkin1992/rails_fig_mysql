# Use docker & fig in development
1. Install [Docker](https://www.docker.com/) & [Fig](http://www.fig.sh/), if you are using Windows or Mac, you also need to install [Boot2docker](http://boot2docker.io/).
2. `sudo fig up -d db` ( This downloads the MySQL image).
3. `sudo fig run web rake db:setup`
4. `sudo fig up` (This downloads the Ruby image).
5. Open your browser at http://localhost:3000 (if you're using Boot2docker, replace localhost by the output of Boot2docker ip).
