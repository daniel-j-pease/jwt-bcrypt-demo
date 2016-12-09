# jwt-bcrypt-demo

the master branch contains only the skeleton. for solutions, see the branches. in particular refer to 'round2', as it contains many features that 'solution' does not.

once it's forked/cloned:

    npm install

then run

    createdb <your_db_name_here>
    psql -d <your_db_name_here> -f ./lib/schema.sql
    psql -d <your_db_name_here> -f ./lib/seeds.sql    

  create a .env that matches the pgConfig object in lib/db.js
    for example, mine looks like this

      PG_HOST=localhost
      PG_PORT=5432
      PG_DATABASE=dan
      PG_USER=daniel_pease
      PG_PASSWORD=
      SECRET=<put your secret here>

  get into psql and query the database to make sure everything is k
