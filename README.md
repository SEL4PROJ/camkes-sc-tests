camkes-sc-tests
===============

These are tests for the CAmkES scheduling context support.

The following test are included:
 * event-driven: testing an event driven thread.
 * event-driven-donate: testing an event driven thread, sender donates scheduling context to the receiver.
 * periodic: testing a periodic thread.
 * cs-donate: client server scenario, client donates scheduling context to server.
 * cs-nodonate: client server scenario, client and server each have their own scheduling context.
 * mcs-donate: multiple clients, one server, clients donate their scheduling contexts to the server.
 * mcs-nodonate: multiple clients, one server, clients and server each have their own scheduling context.
 * cms-donate: single client, chain of multiple servers, only the client has a scheduling context and it is donated down the chain

This repository also contains the repo manifest for the tests.

To fetch do:

    mkdir camkes-sc-tests
    cd camkes-sc-tests
    repo init -u https://github.com/seL4-projects/camkes-sc-tests.git
    repo sync

