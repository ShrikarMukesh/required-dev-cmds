#disable jenkins from starting up automatically on start up
update-rc.d jenkins disable 5

#enable to jenkins run from start up automatically
update-rc.d jenkins disable 5

#disable docker from running
sudo update-rc.d docker disable 5
