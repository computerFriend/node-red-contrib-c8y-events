# node-red-contrib-c8y-events
A NodeRed node that integrates with Cumulocity to fetch device events

## Installation
run npm -g install node-red-contrib-c8y-events

## Features
Fetches event data & can limit the data based on event type, status, & deviceId

## Usage

### Required inputs:
* cumulocity instance name
* tenant name

### Optional inputs:
* deviceId: limits events data to 1 specific device
* type: filters based on event type
* status: filters based on event status
* pageSize: Defines maximum number of records to return


## Why this module?
This node is part of a series of nodes designed to integrate with the Cumulocity IoT platform.  The long-term goal is to create a complete library of node-red nodes that can pair with Cumulocity (analogous to the AWS & Salesforce node-red libraries).

## What's next?
Optional pagination of results is coming next: This will give users to option to have the node run continuously until all events are returned. This will also include the ability to add a max timeout.

I also want to make it easier to have environment variables stored easily in your NodeRed flow.  Parameters like tenant name, usernames, & credentials should all be stored in one location (vs. hard-coded into each node), so that they can be changed, managed, & protected more easily.  Once I have that figured out, I'll update this node to be compatible with that.
