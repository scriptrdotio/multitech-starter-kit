# MultiTech Quickstart App

This is a sample application to on-board MultiConnect Conduit users allowing them to visualize their gateway data using scriptr.io. It is tailored for the MultiConnect® Conduit<sup>TM</sup> IoT Starter Kit for LoRa® Technology, featuring a dashboard that displays the mDot Box' data feed in real-time.

As you connect more devices to the gateway, you can easily modify this application to implement more complex logic to transform and process the data from these devices, and add more widgets to the dashboard to display the data feed in real-time.

# Features
- HTML dashboard "quickstart-app/view/dashboard.html" with 2 gauges to show luminosity and temperature live data.
- Ingest API "quickstart-app/api/ingest" called by the conduit for every new payload the conduit publishes.
- Installation API "quickstart-app/install/auto.install.scriptr" to install the MultiConnect quickstart app dependencies:
     - The channels needed by the application.
     - A default subdomain for the account.
- Uninstallation API "quickstart-app/install/uninstall.scriptr" to uninstall the MultiConnect quickstart app dependencies set by the installation API.
-  Simulator API "quickstart-app/simulator/conduit/data" to simulate the conduit calls to the quickstart-app/api/ingest API.

# How to View the Dashboard

The installation API "quickstart-app/install/auto.install.scriptr" needs to be executed once. In case you used the MultiTech Starter Kit's promotion code to register to scriptr.io, this app should have already been checked out and the quickstart-app/install/auto.install.scriptr should have already been executed automatically.

To view the dashboard and visualize your conduit data in real-time from within your scriptr.io IDE, open the "quickstart-app/view/dashboard.html" file and click View.

# Notes

This app provides a simulator that allows you to simulate the data feed from the gateway in order to visualize it on the dashboard. To use it, you can [schedule](https://www.scriptr.io/documentation#documentation-scriptschedulingScriptScheduling) the "quickstart-app/simulator/conduit/data" script on a recurring basis with the time interval of your choice.
