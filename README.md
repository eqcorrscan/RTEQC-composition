# Composition of RTEQC

Files to orchstrate docker set ups for RTEQC. Needs to have the RCET_RTEQcorrscan, RTEQC_api and RTEQ_grafana repositories cloned within this folder.

To run a simulation, change the event id (and other env variables) in the `Albatross_sim.env` file then run:

`docker compose -f simulation-docker-compose.yml --env-file Albatross_sim.env up`

To run a real-time setup (in production) check the env variables in `Albatross_rt.env` and run:

`docker compose -f docker-compose.yml --env-file Albatross_rt.env up`
