# Instructions

 - Start IBM Personal Communication with the configuration specified in ims.ws (supplied in this directory)
 - Start WDG Studio
 - Start  command_enqueue.wal (supplied in this directory) to enqueue new users
 - Start  OnboardBot.wal (supplied in this directory) to add users to IMS

 # Function

 The bot performs the following tasks:
 - Reads Vault credentials to log in to Z system (IMS)
 - Dequeues commands from a queue.  Commands consist of add/update or delete users
 - Connects to  personal communications terminal
 - Runs a macro within the terminal to login to IMS
 - For each dequeued command, run macro within the terminal to add/delete/modify a User
 - Runs a macro within the terminal to logout of IMS
