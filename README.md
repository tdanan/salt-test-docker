# salt-test-docker
Salt in docker env to test salt functionalities:

run:
 docker-compose -f salt-compose.yml up --build

Check all well configured:
 docker exec -it master salt '*' test.ping

 minion:
    True



