Following along from this timestamp in video "Hasura DDN In Action": https://youtu.be/KFRAXnDIgH8?t=3068

# Commands ran

ddn add connector-manifest fx_connector --type cloud --hub-connector hasura/nodejs:v1.2.0 --subgraph app

ddn update data-connector-link fx_connector --subgraph app

ddn add command --data-connector-link fx_connector --name hello --subgraph app

        LOAD  Project
         ADD  Command for source hello, connector fx_connector
                ERROR Invalid ndc definition for source hello, connector fx_connector
9:12AM ERR error adding command: exit status 2# testfxconnector
